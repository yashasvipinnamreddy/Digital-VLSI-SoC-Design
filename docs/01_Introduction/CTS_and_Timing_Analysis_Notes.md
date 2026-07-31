# Clock Tree Synthesis (CTS) and Post-CTS Timing Analysis

---

## Clock Tree Synthesis (CTS)

Clock Tree Synthesis (CTS) is performed after placement to distribute the clock signal from the clock source to every sequential element (flip-flops and latches).

The objectives of CTS are:
- Minimize clock skew.
- Minimize clock latency.
- Balance clock arrival time.
- Improve setup and hold timing.
- Build a reliable clock distribution network.

During CTS:
- Buffers and clock buffers are inserted.
- A clock tree is created.
- The clock reaches all flip-flops with nearly equal delay.

OpenLANE uses TritonCTS to perform Clock Tree Synthesis.

---

## Clock Buffering

Clock buffers are inserted to:
- Drive large fanout.
- Reduce delay.
- Balance the clock network.
- Improve timing performance.

Buffers are selected from the standard cell library.

Example:
```
Clock Source
      |
    Buffer
     / \
 Buffer Buffer
```

---

## Clock Net Shielding

Clock nets are sensitive to noise because they switch continuously.

Clock shielding:
- Reduces coupling noise.
- Reduces clock jitter.
- Improves signal integrity.
- Provides stable clock distribution.

---

## CTS Configuration Parameters

Some important CTS parameters are:

- CLOCK_PORT
- CLOCK_PERIOD
- CTS_ROOT_BUFFER
- CTS_CLK_BUFFER_LIST
- CTS_MAX_CAP
- CTS_MAX_TRAN
- CTS_TARGET_SKEW

These parameters control how the clock tree is generated.

---

## Running CTS in OpenLANE

During CTS OpenLANE:

- Reads the synthesized netlist.
- Inserts clock buffers.
- Generates the clock tree.
- Creates the CTS DEF file.
- Produces timing reports.

Output files include:
- CTS DEF
- Clock tree reports
- Timing reports

---

## Post-CTS Timing Analysis

After CTS, timing analysis is performed again because:

- Clock delays have changed.
- Clock skew is now realistic.
- Setup timing is recalculated.
- Hold timing is recalculated.

The timing report now includes:

- Clock network delay
- Clock latency
- Data arrival time
- Data required time
- Slack

---

## Interpreting Slack

Slack indicates whether timing requirements are satisfied.

- Positive Slack → Timing Passed
- Zero Slack → Critical Path
- Negative Slack → Timing Violation

Examples:

Slack = +4.48 ns
→ Timing Met

Slack = -0.77 ns
→ Timing Violated

---

## Setup Analysis After CTS

After CTS:

Setup Slack =
Data Required Time − Data Arrival Time

If Slack > 0
→ Setup timing passes.

If Slack < 0
→ Setup violation occurs.

---

## Hold Analysis After CTS

Hold analysis checks whether data changes too early.

Requirement:

Data Path Delay > Hold Time

If data reaches too early:
- Hold violation occurs.

If data reaches after hold time:
- Hold timing passes.

---

## Summary

Flow after Placement:

Placement
↓
Clock Tree Synthesis (CTS)
↓
Clock Buffer Insertion
↓
Clock Net Shielding
↓
Post-CTS Setup Analysis
↓
Post-CTS Hold Analysis
↓
Timing Reports

CTS improves clock distribution and helps achieve reliable setup and hold timing before routing.
