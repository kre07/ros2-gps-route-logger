# Project Structure

- `gps_tracker/route_logger.py` — subscribes to `/gps/fix`, converts latitude/longitude to a local X/Y path relative to the first GPS fix, publishes the accumulated route on `/gps/path`, and appends raw GPS coordinates to `~/MORSEPASSWORD.txt`.
- `gps_tracker/fake_gps.py` — publishes a fixed sequence of simulated GPS waypoints to `/gps/fix`.
- `gps_tracker/ip_gps.py` — obtains an approximate IP-based location, generates a small synthetic square path around it, and publishes those points to `/gps/fix`.
- `README.md` — original project documentation supplied with the source.

This repository is a cleaned GitHub snapshot of the provided route-logging source files.
