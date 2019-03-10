# Notes
## Setting ailerons to max. reflex
<https://www.rcgroups.com/forums/showthread.php?2578134-F3K-program-for-Taranis-QX7-and-X9D-with-scripts-for-score-keeping-and-graphing/page29>

Hello,

is there a way how to set flaperons up for Launch and Zoom flight mode?
Would be nice to have that on throttle trim.

Thank you,
Martin

------

I've already figured it out 
Code:
I5: CbPS   TrmT Weight(+50%) Flight modes (Launch, Zoom, Speed) NoTrim [CambPset]
           TrmT Weight(+50%) Diff(-100) Flight modes (Cruise, Float, FM5, FM6, FM7, FM8) NoTrim [CambPset]
Cheers,
M;

------

It looks like you have copied the camber preset and disabled the -100% differential for Launch, Zoom, and Speed modes. This will allow you to push up the flaperons to have more reflex in those modes with positive throttle trim values. But you should have adjusted the flaperons to max. reflex in the 3rd configuration submenu. The reason why I have set it up this way, is that you will hose the Snap Flap response with positive throttle trim values.

Jesper

------

Jesper,

thanks for reply. I have difficulties to understand max. reflex and 3rd configuration submenu purpose. Could you explain in other words?

Thank you,
M;

------

Max. reflex is the flaperon position that you want for Speed, Launch, and Zoom. For many planes, flaperons are flush with the trailing edge, but for some planes, it is 1-2mm up. 

By setting the max. reflex position in the 3rd config submenu, you allocate the servo travel needed for flaps, and the remaining travel goes to aileron. So full air brake is 100% down. And in e.g. Speed mode without air brake, max. aileron up is 100% up.

Jesper
