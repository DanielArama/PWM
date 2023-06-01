# PWM
* period time (T_done) = (T_clk_100M)*(F_V+1)
* period time (T_PWM) = (2^R)*T_done = (2^R)*(T_clk_100M)*(F_V+1)
* duty cycle (duty) = (duty[R:0]/2^R[R-1:0]

PWM model takes an input clock signal, duty cycle, and final value for counting.
It uses registers and logic to generate a PWM waveform with the specified duty cycle and frequency.
The Timer_PWM module handles the counting and timing aspects to produce the desired PWM signal.
