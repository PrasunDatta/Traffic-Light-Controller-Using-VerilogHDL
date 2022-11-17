# Traffic-Light-Controller-Using-VerilogHDL
This work is the final project of the sessional course - "EEE 304: Digital Electronics Laboratory". In this work, we have implemented a 4 way traffic controller system.
## Brief Overview
<p align ="justify">
There are 8 lanes and at most one way is opened for safely passing the vehicle. When one of the
four junctions is signaled green vehicles can pass from that side to all together three sides. The
illustration for the junction is drawn here. </p>

<p align ="justify">
The green light will be turned on for 8 clock cycles, the yellow light will be turned no for 4 clock
cycles and the remaining 32 clock cycles will be for red. Before turning green from red the light
will become yellow for 4 clock cycles again. Thus, the color switching sequence for a particular
side is, green-yellow-red-yellow- green. The sequence with clock cycle is shown in the table
below. </p>
<b>Color Switching Sequence: </b>
Green -> Yellow -> Red -> Yellow -> Green -> go on

<b> Clock Cycles: </b> 8 clk cyc -> 4 clk cyc -> 32 clk cyc -> 4 clk cyc -> 8 clk cyc -> go on.
<p align ="justify">
The system will start when reset, and enter the north state and start giving output on the negative
edge of reset signal. From the north state, it will go to the next state and keep going. We have
defined 8 states in this design. The states are specified in the table below.</p>
