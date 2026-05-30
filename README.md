# A350-FlightSim
A350 FLIGHT SIMULATOR
# A350-900 Web Simulator

An early open-source Airbus A350-900 style flight simulator for the web.

This first build runs as a static Three.js app and includes a procedural A350-900 placeholder, runway environment, basic flight physics, HUD, throttle, flaps, and landing gear.

## How To Download?

just do
```bash
git clone https://github.com/Liamsitbon/A350-FlightSim.git
```

## Run locally

```bash
python3 -m http.server 5173
```

Then open:

```text
http://localhost:5173
```
(If you pull a new version then you need to change 5173 to a different number each time.)

## Controls

- `W` / `S`: throttle
- Arrow down / up: pitch up and pitch down
- Arrow left / right: roll left and roll right. Holding the key keeps rolling; releasing keeps the bank instead of snapping level.
- `A` / `D` or `Q` / `E`: rudder yaw left and right
- `K` / `I`: climb and descend
- `J` / `L`: bank and turn
- `G`: landing gear
- `Space`: brakes
- Left panel: throttle, flaps, gear
- Right flight pad: pitch, roll, and yaw
- Camera pad: pan around the aircraft and zoom in/out

The aircraft now uses attitude rates for pitch, roll, and yaw, so the controls change the aircraft's motion instead of playing a fixed animation. Weather wind and turbulence also affect the flight path.
