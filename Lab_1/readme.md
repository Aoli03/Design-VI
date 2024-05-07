# Lab 1 -- GHDL and GTKWave Practice
**Using vhdl entity and testbenches, make use of both GHDL and GTKWave as a wave visualizer.**

<hr>

### Half Adder
You begin by usign GHDL to analyze the two files, a testbench and a top entity of the half adder, and eventually execute the testbench.
After gathering the outputs as a function of time, we can run the GTKWave file.

![Command Prompt Input](Figures/Half_Adder_Setup.png)

A half adder should sum two bit values: `a` and `b` here.
The results will go into the sum, or the carry bit, represented by `s` and `c`, respectively.


Below `a=0` and `b=0` so both `s=0` and `c=0`:

<img src="Figures/HA_GTKWave_1.png" alt="System State 1" width="700" height="350"/>

Below `a=0` and `b=1` so both `s=1` and `c=0`

<img src="Figures/HA_GTKWave_2.png" alt="System State 2" width="700" height="350"/>

Below `a=1` and `b=0` so both `s=1` and `c=0`

<img src="Figures/HA_GTKWave_3.png" alt="System State 3" width="700" height="350"/>

Below `a=1` and `b=1` so both `s=0` and `c=1`

<img src="Figures/HA_GTKWave_4.png" alt="System State 4" width="700" height="350"/>

This represents the four states that the half-adder system can have!
This system is asynchronous from any clock and responds immediately to internal change.

<hr>

### D-Flip Flop
You begin by usign GHDL to analyze the two files, a testbench and a top entity of the D-Flip FLop, and eventually execute the testbench.
After gathering the outputs as a function of time, we can run the GTKWave file.

![Command Prompt Input](Figures/DFlip_Flop_Setup.png)

**D-Flip Flop:** The premise of a D-Flip Flop is to take input on the `din` line, and whatever is present on the _rising edge_ of the clock \[From 0 --> 1\] will be retained as output until the next _rising edge_, acting as memory for one clock cycle.

The reset signal, or `rst`, is used to make the output go back to `dout=0` if `rst=1`, asynchronously from the clock, as long as it is held at 1.
After letting go, `rst=0`, the flip flop goes back to normal operation on the next _rising edge_.

Below, you can see that `din` was equal to zero on the last rising edge, and so `dout` is also retained as `0`.

<img src="Figures/DFF_GTWave_1.png" alt="System State 1" width="700" height="350"/>

Below, you can see that `din=1` starting from the falling edge, and so `dout=0` until the rising edge, where you see that `dout` becomes `1`.

<img src="Figures/DFF_GTWave_2.png" alt="System State 2" width="700" height="350"/>

Below, you can see `din=1` is being held, however, on a  _falling edge_ `rst=1` begins to be held, so `dout` is forced to be `0`, against any input.

<img src="Figures/DFF_GTWave_3.png" alt="System State 3" width="700" height="350"/>


