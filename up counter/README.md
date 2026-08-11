# 4-Bit Up Counter using Verilog

## 📌 Project Description

This project implements a **4-bit synchronous up counter** using Verilog HDL.

The counter increments its value by 1 on every positive edge of the clock. When the reset signal is high, the counter is reset to `0000`.

## 🛠️ Features

* 4-bit up counter
* Synchronous reset
* Positive-edge triggered
* Counts from `0` to `15`
* Verilog HDL implementation
* Testbench included
* Simulation waveform included

## 📂 Project Files

| File                      | Description           |
| ------------------------- | --------------------- |
| `up_counter.v`            | Verilog design code   |
| `up_counter_tb.v`         | Testbench             |
| `simulation/waveform.png` | Simulation waveform   |
| `README.md`               | Project documentation |

## 🔢 Working

When `reset = 1`, the counter output becomes:

```text
0000
```

When `reset = 0`, the counter increments on every positive clock edge:

```text
0000 → 0001 → 0010 → 0011 → ... → 1111
```

After `1111`, the 4-bit counter rolls over to:

```text
0000
```

## 🧪 Simulation

The testbench generates a clock with a 10 ns period and applies reset initially.

Expected output:

```text
Time = 0  | Reset = 1 | Count = 0
Time = 15 | Reset = 0 | Count = 1
Time = 25 | Reset = 0 | Count = 2
Time = 35 | Reset = 0 | Count = 3
...
```

## 💻 Tools Used

* Verilog HDL
* Icarus Verilog / ModelSim / Vivado
* GTKWave

## 🎯 Applications

Up counters are commonly used in:

* Digital clocks
* Frequency counters
* Timers
* Digital systems
* Control circuits
* FPGA-based projects

## 👩‍💻 Author

**Rowthu Shiva Naga Poojitha**

## 📜 License

This project is created for educational purposes.
