# Voron0-TinyM-
An older Voron0 like project that I am rebuilding from the ground up.

Old version left-side, new version right-side (still under construction)

<p float="left">
  <img src="https://github.com/user-attachments/assets/4441eda1-e2fe-4d38-ae90-1ebbe2facb45" width="320" />
  <img src="https://github.com/user-attachments/assets/264cd8ba-e761-49a3-9ffa-67f99cb4d31b" width="440" /> 
</p>

The older design was a Voron0, TinyM configuration (meaning the main frame is made of 2020 extrusions over the 1515 default ones, and all relevant hardware changed to match this),
furthurmore, I used a 100x100mm print bed with 4 corner levelling, a klicky probe (https://github.com/jlas1/Klicky-Probe), bowden extruder, octopus pro board and an old ender3 power supply.

This setup worked well in some aspects. 
- It could achieve very high speeds (40k accel, at 450mm/s with motors at 1.2a and 24v)
- Heated up extrordinairly quickly (bed heated in 17 seconds to 70C [RXL heats in ~5 minutes]),
- Was fully enclosed (helped with noise and heated chamber)
- Very compact (everything fit within the dedicated frame, except the extruder)
  
However, Some things did not work well:
- The 4 point levellng of the bed overconstrained it (3 points make a plane, 4 points bend it)
- The bed warped severely due to its 2.5mm thickness, but 250W heating power.
- The klicky probe, 4 point levelling, bed meshing, and overall software related tuning for the first layer was not done properly (this combined with the above points made first layers extremely inconsistent).
- Colour cordination and asthetics were non existant (parts were printed out of whatever colour was nearby [photo has parts from 7 different filaments in it])  

Breakdown of the printer right before being dismantled (please note many of the changes I mentioned in the video are no longer relevant, this github has the true design goals): https://youtube.com/shorts/kxB7ypKhO4k
Random Printing video I had on hand: https://youtube.com/shorts/vAiskhb0QYo?feature=share
Many parts of the older build went to the RXL printer including the 24v 15a power supply, Octopus Pro board, TMC2209 motor drivers, Custom Hotend, etc.


The NEW design immediate changes (project started November 1st, goal is functioning by Mid december)
- 2040 extrusions on corners
- Aluminum braces at front and back (will act as reinforcment and also help square the frame)
- New build volume (120mm x 120mm(+20mm) x 115mm [extra room for nozzle wiper on Y])
- Proper 8mm superflat Aluminum MIC6 voron0 bed (no more warping, however takes ~3mins too heat up)
- Colour cordinated parts (Black and Blue themed, with 2020 slot inserts)
- Higher flow hotend (34.5mm to 42.5mm melting zone [up to 70mm/s3])
- Orbiter direct drive extruder (option to use it for bowden, but will greatly help quality either way)
- Compact fanless 24v power supply (Reduces noise and leaves more room in electonics bay)
- better printer feet (same as RXL)
- Camera to monitor prints
- 3 point bed levelling 
  
Later updates:  
- Enclosure (acrylic needs to be cut down)
- Tulip Mod (not sold on the benefits of this yet, so this mod is a maybe)
- Screen added.
- 100mmx100mm super fast bed switchout ability?
- Conveyor for print bed switching


Since this printer will act as a secondary option to my RXL, many design goals are the same, and based on the success of the RXL.
Since many of the physical changes have been listed above, below will be more functionality related goals:
- Same print speeds as RXL (will be tuned to reach much higher speeds later on)
- Same absolute reliability (+99%, this printer should be a "print & forget" style)
- Complete wire managment
- Fully enclosed and able to print ABS flawlessly.
- Quiet at high speeds (if possible)


Rebuild started: November 1.  
First print: December 7.  
Current updates and next steps:  
 - All cable managment done and very clean (for now)  
 - Already very reliable, with perfect first layers, and good print quality.  
 - Currently have it printing about 10% faster than RXL, but will be tuning to continue increasing speed.  
 - Nozzle wiper, purge shoot and electronics pannels to be printed next.
 - Pi Camera to be added
 - 



Speed Testing 
|  AB Motor Power  | Par1 -> Par2(at step loss)  |  Notes  |
|       :-----:         |       :---:      |
|  24v@0.8a  | 10k -> 600mm/s  | remarkably quiet  |
|  24v@0.8a  | 20k -> ?mm/s  | ...   |
|  24v@0.8a  | 30k -> ?mm/s  | ...   |
|  24v@1.41a  | 20k -> ?mm/s  | ...   |
|  24v@1.41a  | 30k -> ?mm/s  | ...   |
|  24v@1.41a  | 40k -> ?mm/s  | ...   |
