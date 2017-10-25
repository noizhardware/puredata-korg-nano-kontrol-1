# puredata-korg-nano-kontrol-1
### _nanok_

## Abstraction for Korg Nano Kontrol 1


This abstraction sends data from the Korg Nano Kontrol version 1 in the format **_s(scenenumber)[letter][number]_**

[letter] is: **b**=button **f**=fader **p**=potentiometer

e.g.:

-s1b3 is button 3 of scene 1

-s2f4 is fader 4, scene 2

-s3p5 is potentiometer 5, scene 3

Scene 4 has hardware built-in latching buttons, nanok sends 0/1 toggle values, according to the hardware on/off LEDs

bg = Button Gate, sends a "1" until the key remains pressed, a 0 when it´is unpressed

e.g.:

-s1bg3 is the gate for button 3, scene 1
