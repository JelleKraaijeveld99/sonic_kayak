This project is a framework devoloped by students of the HKU Creative System Design year 2023 named Sonic Echoes. We made a audio immersive journey that is bound by GPS locations near Uncloud Utrecht.

In this repository you can find documentation on the pure data patches we made that we build on the Sonic Kayak and Sonic Bike repos.

We recommend recreating the image for the SD card of the PI before implementing the PD patch in the System.

Link to the repos:
Sonic Bike: https://github.com/sonicbikes/sonic-bike-init
Sonic Kayak: https://github.com/fo-am/sonic-kayaks

In short how the system runs.

1. When the PI starts, the sonic-bike.service will load all the nessecairy things in the background (sensors etc.). This is done with SWAMP. Swamp will also load a headless (--nogui) version of the .pd patch located at: home/pi/stick/sonickayak/pd/sonickayak.pd this is done via the shells script home/pi/app-kayak/audio_restarter/start_jack.sh

2. If you want to start the .pd patch with gui: home/pi/app-kayak/audio_restarter/gui_start_jack.sh , now you can modify the patch and save it, so you can create your own patch.  
