# friendly-potato

I wanted to test the 7 segment display on my Spartan6 devboard and whipped this up. I drive a counter from the 50MHz xtal and show the upper 16 bits of the counter in realtime. Button 1 resets the counter and button 2 disables the anode drivers which blanks the display.

The sseg entity sequences through the digits of the captured value with each rising clock edge fed to it. The value to display is also captured automatically on the same edge.

I experimented with trying to do a state machine in a more logical manner (to me). I'm **very** happy with how things synthesized --- exactly as anticipated.
