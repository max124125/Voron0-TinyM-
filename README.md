# Voron0-TinyM-
An older Voron0 like project that I am rebuilding from the ground up.

The older design was a Voron0, TinyM configuration (meaning main frame is made of 2020 extrusions over the 1515 default ones, and all relevant harder changed to match this),
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


The NEW design changes:
- New build volume (120mm x 120(+20)mm x 115mm) 
