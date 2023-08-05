# Solar-Powered LED Flashlight Business Card
created by Colin Catlin, 2023

A business card that can also double as a decently powerful, RGB flashlight, complete with solar charging. Built for business, ready for the apocalypse.

Built in KiCAD V6, opens with V7 and possibly later (those haven't been released as of this release).

GPLv3 licensed so that you can freely go and make variations with your own name. Or run around handling out ones with my name while pretending to be me? Please only do the latter if you are very charming and attractive.

I have had this made and assembled by JLCPCB, as you'll notice. Only the back side was assembled by them. 
Additionally there is a PTC reset fuse which is marked with a 0 ohm resistor, size 1812. 
You can use the resistor if you don't want the reset fuse, it isn't necessary but adds a little extra safety.

For that fuse, I chose Bourns MF-MSMF020-2 PTC RESET FUSE 30V 200MA 1812 and hand-assembled it with hot air. It's a relatively big part, easy to solder.

I also hand assembled the solar panel and the LEDs on the front side. Choosing LEDs is fun. I tried to size the pad so that that most 3030 or 2835 LEDs would work. 
I found that it even works with those that have a three part footprint (one of which can safely be connected to return). 

The giant vias are for allowing hot air from the bottom to reach solder paste on the other side for attaching the solar panel. It works. Actually these vias are bigger than really necessary, going down a bit smaller would work well and be more discrete, but not too small, 0.3 mm was definitely too small.

The idea here with three LEDs is that you can choose three different colors, red, green, and blue, and then mix them with potentiometers to make 'any' color. It works! 
But for more flashlight purposes you can just choose the most efficient white-ish colors (for still some fun, choose a low kelvin and high kelvin color mix, so you still can get blue-ish and yellow-ish). I had thought the Samsung ultra efficient LEDs would be best, and they do work well, but for the best flashlight I found the narrowest possible viewing angle made the most impact (since there is no light focusing reflector here like a normal flashlight). One I tried that worked well was the "LED Lighting OSLON® SSL 80 White, Cool 6500K 2.85V 350mA 80° 1212 (3030 Metric)" - the most important part is that 80 degree viewing angle.

The idea here was the undervoltage protection would be afforded by the dropout voltage of the LEDs (they stop working with too little voltage, that's good here). Unfortunately I have found that green LEDs, in particular, can run down to a lower voltage than their datasheet suggests. Check the minimum voltage of LEDs manually if aiming for optimal battery protection.

Please see my blogpost for more details: 
https://syllepsis.live/2023/08/05/the-solar-powered-business-card/
