
# PLL Example

This example does the following:
* LED1 is connected to the ```blink``` block from the ```blink``` example and uses the regular 100MHz input clock.
* LED2 is also connected to the ```blink``` block but it uses a clock that is generated by a PLL.
* The PLL is generated with ```icepll``` tool from the Project IceStorm toolset, and is configured to generate
  a 30MHz clock out of a 100MHz input.

    Check out the Makefile to see how theh pll.v file is generated with the ```icepll``` tool.

After uploading the design to the board, you should see LED1 (red) blink at 3 times the frequency of LED2 (orange.)

More information about PLLs can be found on the [PLL wiki page](https://github.com/mystorm-org/BlackIce-II/wiki/PLLs).
