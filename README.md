Kartduino
=========

FAQ:
=========

Q: Kartduino, clever name. Does it mean anything?

A: Initial aim was for a simple DIY ECU for go-karts. The important part of that being SIMPLE! The code is written with simplicity above all else in mind and all areas are well commented. The project can be loaded directly into the Arduino IDE and compiled with only a single additional library needing to be added. Where code is complex or low level, a high level pseudo code example is given to explain what is being performed. 

========================================================================

Q: Arduino ECU,pffft, heard THAT before. Does this one actually work?

A: Yep! Single cylinder engines are well tested and working as of Nov 2013. Final work continues on accleration enrichment and will then move onto multi-cylinder engines early in 2014

========================================================================

Q: So what can it do?

A: Initial plan is for injection and ignition control on single cylinder 4 stroke engines. 
Features:
* 8x8 maps with interpolation
* Support for missing tooth crank wheels up to 36-1 with hall effect sensor
* Alpha-N or Speed Density load control
* High-Z injector hardware
* Warmup enrichment
* Acceleration enrichment
* Compatible with Tuner studio (http://tunerstudio.com/) for tuning

Phase 2 will include:
* Batch support for up to 4 cylinder engines
* 2 stroke engine support
* Closed loop EGO / O2 
* Autotune with TunerStudio and wideband O2

========================================================================

Q: Target platform?

A: Arduino Mega (Or other ATmega1280 / ATmega2560 powered SKU) will be required. Standard arduino models are not suitable for multi-cylinder engines due to their lack of 16-bit timers. The shield board has been designed around the Mega and it is not expected that there will be a non-Mega variant. 
