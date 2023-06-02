# PWM
* period time (T_done) = (T_clk_100M)*(F_V+1)
* period time (T_PWM) = (2^R)*T_done = (2^R)*(T_clk_100M)*(F_V+1)
* duty cycle (duty) = (duty[R:0]/2^R) ( To set a 100% duty cycle, you need to assign the maximum value to the duty input.
 Since R is 8, the maximum value is 2^8 - 1 = 255. However, a value of 256 should be used for 100% duty cycle.
Therefore, to achieve a 100% duty cycle with R set to 8, you should set the duty input as follows: "duty = 256;" )

PWM model takes an input clock signal, duty cycle, and final value for counting.
It uses registers and logic to generate a PWM waveform with the specified duty cycle and frequency.
The Timer_PWM module handles the counting and timing aspects to produce the desired PWM signal.
