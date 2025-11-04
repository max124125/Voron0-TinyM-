# Voron0-TinyM-
An older Voron0 like project that I am rebuilding from the ground up.

Old version left-side, new version right-side (only a partial CAD until physical frame constructed).

<p float="left">
  <img src="https://github.com/user-attachments/assets/4441eda1-e2fe-4d38-ae90-1ebbe2facb45" width="350" />
  <img src="https://github.com/user-attachments/assets/2802e226-4814-4c2b-bfb2-39cb0906b758" width="352" /> 
</p>



The older design was a Voron0, TinyM configuration (meaning the main frame is made of 2020 extrusions over the 1515 default ones, and all relevant harder changed to match this),
furthurmore, I used a 100x100mm print bed with 4 corner levelling, a klicky probe (https://github.com/jlas1/Klicky-Probe), bowden extruder, octopus pro board and an old ender3 power supply.

This setup worked well in some aspects. 
- It could achieve very high speeds (40k accel, at 450mm/s)
- Heated up extrordinairly quickly (bed heated in 17 seconds to 70C [RXL heats in ~5 minutes]),
- Was fully enclosed (helped with noise and heated chamber)
- And very compact (everything fit within the dedicated frame
- 
However, Some things did not work well:
- The 4 point levellng of the bed overconstrained it (3 points make a plane, 4 points bend it)
- The bed warped severely due to its 2.5mm thickness, but 250w heating power.
- The klicky probe, Z motor tuning, and overall software related tuning was not done properly (this combined with the above points made first layers extremely inconsistent).
- Colour cordination and asthetics were non existant (parts were printed out of whatever colour was nearby)


The NEW design immediate changes (goal: functioning by end of November)
- 2040 extrusions on corners
- Aluminum braces at front (will act as reinforcment and also help square the frame)
- New build volume (120mm x 120mm(+20mm) x 115mm [extra room for nozzle wiper on Y])
- Proper 8mm superflat Aluminum MIC6 voron0 bed (no more warping, however takes ~3mins too heat up)
- Colour cordinated parts (Black and Blue themed, with 2020 inserts)
- Higher flow hotend (34.5mm to 42.5mm melting zone [up to 70mm/s3])
- Orbiter direct drive extruder (option to use it for bowden, but will greatly help quality either way)
- Compact fanless 24v power supply (Reduces noise and leaves more room in electonics bay)
- better printer feet

Changes later on (In order of priority)
- 3 point bed levelling (new mainboard needed though)
- Enclosure (acrylic needs to be cut down)
- Tulip Mod (not sold on the benefits of this yet, so this mod is a maybe)
- Screen 
