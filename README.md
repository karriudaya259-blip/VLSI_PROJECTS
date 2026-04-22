# Synchronous FIFO (Parameterized)

## Description
A First‑In‑First‑Out buffer with configurable depth and width.  
Flags: `full`, `empty`, `almost_full`, `almost_empty`.  
Uses a counter to track number of stored words.

## Files
- `fifo_sync.v` – design
- `fifo_sync_tb.v` – testbench (dumps VCD)
- `waveform.png` – GTKWave screenshot

## How to simulate
```bash
iverilog -o fifo.vvp fifo_sync.v fifo_sync_tb.v
vvp fifo.vvp
gtkwave fifo.vcd
