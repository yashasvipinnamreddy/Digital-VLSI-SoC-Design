# Clock Tree Synthesis (CTS)

## Objectives
- Reduce clock skew
- Minimize clock latency
- Balance clock paths
- Insert clock buffers

## CTS Configuration
- Clock period
- Clock port
- Clock buffer list
- Root buffer
- Target skew
- CTS tolerance

## Buffer Insertion
- Clock buffers are inserted to balance the clock tree.
- Fanout is reduced using multiple buffer levels.

## Clock Net Shielding
- Shields clock wires from signal noise.
- Improves clock integrity.

## CTS Reports
- Number of clock buffers
- Clock nets created
- Clock skew
- Clock latency

## Timing after CTS
- Use propagated clocks.
- Re-run setup timing.
- Check slack after CTS.
- Replace buffers if needed to improve timing.
