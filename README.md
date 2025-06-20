# 16-to-1 Multiplexer in Verilog

This repository contains the **behavioral Verilog implementation of a 16-to-1 multiplexer**, along with a **testbench** and waveform file generated using simulation tools. It is a great starting point for anyone learning digital design and HDL simulation.

## 📁 Files

- `mux_beh.v` – Behavioral Verilog code for 16-to-1 multiplexer
- `mux_beh_tb.v` – Testbench for simulating the multiplexer
- `mux16to1.vcd` – Waveform output (VCD file) for GTKWave analysis
- `mux_beh_out` – Output file (optional: simulation result/log)

## 🧠 Overview

A **16-to-1 multiplexer** has 16 data inputs and 4 select lines. Based on the binary value of the select lines, one of the 16 inputs is routed to the output.

## 🛠️ Tools Used

- **Icarus Verilog** – for compiling and running Verilog code
- **GTKWave** – for viewing simulation waveforms

## ▶️ How to Run

### 1. Compile

iverilog -o mux_sim mux_beh.v mux_beh_tb.v

2. Simulate

vvp mux_sim

###3.WaveForm

gtkwave mux16to1.vcd

###TestBench Highlights

Applies different combinations to the sel (4-bit) input

Drives 16 input lines with test values

Verifies the output corresponds to the selected input

Generates a VCD file for waveform analysis
