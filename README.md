# LUA nodemcu implementation of an attic thermometer + relay with web config

So, this was my attic thermostat control -- the first version.
It was done in NodeMCU LUA, which I gave up on after a while due to some
memory leaks that seemed to be in the firmware.  (I moved to doing it all
in Arduino C, and things went smoother from that point on.)
That was 2 years ago and the memory issues might be resolved.  Nevertheless,
I've not tried to use this project since then, and it likely won't work
fresh out of the box.  I'm putting it online as reference for a friend, and
in case anyone else finds it useful, but it likely won't work "out of the box".
(It also depends on the ds18b20 module.)

## To use, aside from other potential dependencies (again, it's been a while):

1. Copy cfg.lua.default to cfg.lua and edit it :)
1. Also, edit w_home.lua, if you're using OTA (over the air) updates, for the form's IP destination
1. The Makefile has various luatools commands to install the files to the device, and I'm not sure if it all works anymore.
