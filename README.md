## Hi, I'm Ajeeth 👋

**MSc Microelectronics student at TU Delft** working on digital IC design: RTL, verification and physical design.
I take designs from SystemVerilog all the way to a signed-off layout, and I like finding out *why* a path is slow before changing anything.

Before this MSc I completed an MSc in Power Electronics at TU Delft (published thesis) and spent four years as a hardware engineer at Dow, where every failure needed a root cause.

📍 Delft, the Netherlands · 🔎 Looking for a **2027 internship or MSc thesis** in CPU design, verification or physical design

---

### 🔧 Featured projects

#### [RV32I 5-stage pipelined CPU: RTL to GDSII](https://github.com/Ajeeth93/riscv32i-5stage-pipelined-cpu)
SystemVerilog RISC-V core with full forwarding, load-use stalls and branch flushing, verified with a self-checking testbench and a UVM environment, then taken to a signed-off layout in **SkyWater 130 nm** with LibreLane.

| | |
|---|---|
| Sign-off | **55.6 MHz**, 0 setup/hold violations at **9 PVT corners**, DRC/LVS clean |
| Optimisation | Critical path traced with STA + SDF gate-level simulation; dedicated branch comparator → **Fmax +22 %**; utilization sweep → **die −42 %** (0.123 mm²) |
| Verification | UVM: 1,170 transactions, 0 mismatches, **99.21 % coverage**; gate-level simulation with SDF at slow and fast corners |
| Explore | **[Interactive layout viewer](https://ajeeth93.github.io/riscv32i-5stage-pipelined-cpu/layout/)**: zoom from the whole die down to single transistors |

#### [16 KiB direct-mapped write-back cache](https://github.com/Ajeeth93/direct-mapped-writeback-cache)
Write-back, write-allocate cache controller (1,024 lines × 128 bit) with valid/ready CPU and memory interfaces. Self-checking testbench with a latency memory model: 13 directed tests and 1,000 random accesses, 0 mismatches. 100 MHz on Zynq-7000.

#### [MIPS 5-stage pipelined CPU](https://github.com/Ajeeth93/MIPS-5stage-pipelined-cpu)
Five-stage pipelined MIPS processor in Verilog.

---

### 🛠️ Tools and skills

| Area | |
|---|---|
| RTL design | SystemVerilog, Verilog · pipelined datapaths, hazard and forwarding logic, FSMs, valid/ready interfaces |
| Verification | UVM 1.2, self-checking testbenches, reference models, constrained-random stimulus, functional coverage, gate-level simulation with SDF |
| Physical design | LibreLane (Yosys, OpenROAD, OpenSTA, Magic, KLayout, Netgen) · Cadence Genus, Innovus, Tempus · multi-corner STA, IR drop, DRC/LVS |
| FPGA | Xilinx Vivado, Zynq-7000, AXI |
| Scripting | Python, Tcl, Bash · C (working knowledge), C++/CUDA (coursework) |

### 🚧 Currently working on
- Integrating my cache with the RISC-V core, with SRAM macros and a clean-room rebuild of the physical-design flow
- The same CPU through the Cadence flow (Genus, Innovus, Tempus) for a tool comparison

### 📫 Contact
[LinkedIn](https://www.linkedin.com/in/ajeeth-phrassanna)
