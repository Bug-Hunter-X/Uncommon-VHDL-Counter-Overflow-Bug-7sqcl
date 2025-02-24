# Uncommon VHDL Counter Overflow Bug

This repository demonstrates a subtle bug in a VHDL counter implementation.  The counter is designed to count from 0 to 15 and then reset.  While seemingly functional, its behavior might not be what is expected in all scenarios.

The bug lies in the way the counter handles overflow.  The current implementation abruptly resets to 0, which might lead to unexpected behavior if the counter needs to wrap around to 0 continuously or if the reset condition is not properly managed.

This repository also provides a solution that addresses the potential problems.