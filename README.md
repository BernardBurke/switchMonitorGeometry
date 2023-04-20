# switchMonitorGeometry
For 3 screen linux system, map the offsets to different screen numbers

I've had numerous experiences of 3 screen linux machines that will somehow 'change' the x windows display number after a sleep, reboot etc.

With Mint, the Display Numbers behave themselves (so that Left to Right mouse navigation works as expected.. however, programs that point at an X-windows screen number (like mpv --screen=2 for example), will behave a little unpredictably after a sleep or upon a reboot).

So, instead of trying to change X display numbers (or mess with xorg.conf), I use txt files that contain the HxW+Xoffset+Yoffset)...

.. it occurred to me that this might tbe place to create a 'switch', which can be implemented as a pair of git branches...as there are two scenarios.

Branch X-Display Right to Left - (called RTL)
Branch X-Display One and Two swapped (called O2S)

There are currently 12 text files,6 of them change as a 'set.
