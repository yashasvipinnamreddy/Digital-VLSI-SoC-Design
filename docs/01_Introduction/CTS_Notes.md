# Clock Tree Synthesis (CTS)

## Clock Tree Synthesis

Clock Tree Synthesis (CTS) distributes the clock signal from the clock source to all flip-flops with minimum skew and delay.

Goals:
- Reduce clock skew
- Minimize clock latency
- Balance clock paths
- Reduce clock power

---

## Clock Buffers

Clock buffers are inserted to strengthen the clock signal and drive large loads.

Benefits:
- Reduce delay
- Improve signal integrity
- Balance clock distribution

---

## Power Aware CTS

Power Aware CTS optimizes the clock network while reducing power consumption.

Key ideas:
- Multi-level buffering
- Equal load distribution
- Same buffer type at the same level
- Balanced clock tree

---

## Buffer Delay Tables

Delay depends on:
- Input slew
- Output load

Delay tables help the CTS tool choose the best clock buffer.

---

## OpenLane CTS Configuration

Important configuration parameters include:
- Clock period
- Clock port
- Clock buffer cell
- CTS strategy
- Buffer insertion options

These settings control how the CTS stage is executed.

---

## CTS Results

After CTS:
- Clock buffers are inserted.
- Clock tree is generated.
- Clock skew is reduced.
- Timing is improved.

The generated layout can be viewed in Magic VLSI.

---

## Summary

CTS is performed after placement.

Its purpose is to distribute the clock evenly to all sequential elements while minimizing skew, delay, and power consumption.
