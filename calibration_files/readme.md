Here are some files from Printables that I like to use.

# Calibraton of extruder through put – https://www.youtube.com/watch?v=Mnvj6xCzikM

G91

G1 E50 F60 #extrude 50 mm of filament, it will take 60 seconds

Then continue with increasing the value of F by 60, till the extrusion will be inconsitent or it will start cliking/skipping.
e. g. G91; G1 E50 F120; G91; G1 E50 F180; ...; G91; G1 E50 F300 #which is 5mm/sec

Max volumetric flow rate is mm<sup>3</sup>/s - πr<sup>2</sup> × how much filament is going in (in seconds)
i. g. max flow rate = 3,14 × (1,75/2)<sup>2</sup> × 5 = 12 mm<sup>3</sup>/s

Max print speed is derived/divided from the max. vol. flow rate - layer width × layer height × speed.
Considering nozzle 0.4 mm, that leaves us with 0.4 width a let's go with 0.2 layer height; that results in 0.4 × 0.2 × 50 = 4

Resolution - as long as the extruder can bare 5 mm<sup>3</sup>/s, you can print safely with 0.4 nozzle at 0.2 layer height at speed 50 mm/s.

Another example | thicker layer at 150 mm/s
Let's say I want to go with 0.3 layer height and the first layer will be 0.48 width (all in mm). 0.3 × 0.48 * 100 = 21,6 mm<sup>3</sup>/s.
So the extruder has to be able to proccess 9 mm of filament per second.
