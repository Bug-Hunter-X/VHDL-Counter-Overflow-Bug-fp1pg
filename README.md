# VHDL Counter Overflow Bug

This repository demonstrates a common bug in VHDL code: an integer counter that overflows without proper handling. The original code (`counter.vhdl`) increments a counter without checking for the maximum value.  This can lead to unexpected behavior or simulation errors. The fixed version (`counter_fixed.vhdl`) addresses this by adding a modulo operation to prevent the overflow.

## Bug Description
The `counter.vhdl` design will increment the internal counter `internal_count` even after reaching its maximum value (15). This will cause an overflow, leading to unexpected results. 

## Solution
The `counter_fixed.vhdl` demonstrates a corrected design, handling the overflow by using the modulo operator.  This ensures that the counter wraps around to 0 when it reaches the maximum value, preventing unexpected behavior.
