## How it works

This is a simple 8-bit combinational adder test module. It adds two 8-bit inputs (`ui_in` and `uio_in`) and outputs the low 8 bits of the resulting sum on `uo_out`. The bidirectional I/O pins are configured purely as inputs, and internal unused nets are tied off to prevent synthesis warnings.

## How to test

Set dedicated inputs (`ui_in`) to any 8-bit value and bidirectional inputs (`uio_in`) to a second 8-bit value. Verify on the dedicated output pins (`uo_out`) that the value equals `(ui_in + uio_in) & 0xFF`.

## External hardware

None.