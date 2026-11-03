# Jillian Yang — ASIC Verification Portfolio

Target role: **NVIDIA ASIC Verification Intern — Summer 2027 (JR2027982)**.
### RTL Design · Functional Verification · FPGA · Embedded Systems

Third-year **Electrical Engineering** student at the **University of Toronto**, with a minor in **Artificial Intelligence & Robotics**. I build digital hardware and use reference models, simulation, and system-level testing to check that it behaves as intended.

**Seeking Summer 2027 / PEY opportunities in ASIC verification, RTL, and FPGA engineering.**  
Interested in **SoC memory-subsystem verification** and FPGA–software integration.  
Available **May 2027** for **12–16 months** · Toronto, Canada · Canadian permanent resident; no sponsorship required.

[Portfolio](https://jillian06.github.io/nvidia-asic-verification-portfolio/) · [LinkedIn](https://www.linkedin.com/in/jillian-yang-46356428a/) · [Email](mailto:jillian.yang@mail.utoronto.ca)

---

## Verification & hardware highlights

| Evidence | Result / scope |
| --- | --- |
| Python ↔ SystemVerilog golden-model comparison | **120 multi-length FFT regressions**, bit-exact agreement |
| Adaptive BFP overflow checking | **48 guard tests**, zero observed overflow in those tests |
| Numerical-quality evaluation | **+24.31 dB SQNR** versus fixed per-stage scaling at 35 dB input SNR |
| Cyclone V synthesis | **51.73 MHz**, 456 ALMs, 209 registers, 2 DSP blocks, 49,152 memory bits |
| FPGA integration | VGA timing, FSMs, collision logic, PS/2 input; **22% lower on-chip memory use** |
| Hardware–software validation | Interface specifications, functional testing, STM32 firmware, MMIO, interrupts, SWD debug |

These FFT figures describe the documented research implementation. The [public FFT repository](https://github.com/Jillian06/fmcw-radar-bfp-fft) provides a clean reference model, numerical checks, and research documentation; its public tests have a smaller scope than the original RTL regression environment.

## Research experience

### Configurable FFT Hardware Accelerator for FMCW Radar — University of Cambridge
**Research Assistant · May–September 2026**

- Designed a synthesizable **1024-point radix-2 SystemVerilog FFT** for 10-bit ADC FMCW radar range processing, with configurable precision and stage-wise adaptive block-floating-point scaling.
- Implemented magnitude monitoring, guard-based shift decisions, shared-exponent handling, and fixed-point arithmetic.
- Built a **bit-accurate Python–SystemVerilog verification flow** and evaluated numerical precision, overflow behavior, FPGA timing, and resource trade-offs.
- Reported results include 120 bit-exact regressions, 48 overflow-guard tests, and the synthesis/accuracy figures above.

[Reference model & research documentation](https://github.com/Jillian06/fmcw-radar-bfp-fft) · [Verification scope](https://github.com/Jillian06/fmcw-radar-bfp-fft/blob/main/docs/VERIFICATION.md)

### Hardware Architecture Research — University of Cambridge
**Research Assistant · June–August 2026 · Supervised by Prof. Özgür B. Akan**

- Contributed to digital hardware architecture work covering RTL, computational datapaths, memory organization, and accelerator resource trade-offs.
- Reviewed implementations through **ModelSim waveform analysis**, functional simulation, and iterative refinement using SystemVerilog and Quartus Prime.

### Spiking Neural Networks & Neuromorphic Computing — University of Toronto & York University
**Research Assistant · May–June 2025**

- Analyzed hardware-aware optimization and the mapping of SNN algorithms to constrained embedded/neuromorphic platforms.
- Examined compute, memory, precision, and low-power deployment trade-offs.

[Research notes](https://github.com/Jillian06/neuromorphic-snn-research) — documentation-focused portfolio repository.

### Autonomous Path Planning — University of Cambridge
**Research Assistant · November 2022–February 2023**

- Developed and evaluated enhanced A* path planning, studying heuristic weighting, node expansion, and obstacle-clearance trade-offs.
- Co-authored an **IEEE ICCECT 2023** paper; public code is a clean reimplementation accompanying the published method.

[Research portfolio](https://github.com/Jillian06/safe-astar-path-planning) · [Published paper](https://doi.org/10.1109/ICCECT57938.2023.10141167)

### Biologically Inspired Robotics — University of Cambridge
**Research Assistant · September–December 2022**

- Built MATLAB simulations of bio-inspired locomotion and sensorimotor control.
- Compared neural-controller architectures and adaptive behavior in simulation.

## Work experience

### Software / Test Engineering Intern — Shenzhen Image Technology
**May–June 2025**

- Authored **hardware–software interface specifications** and contributed to system-level validation and functional testing.
- Worked across component interfaces to support integration, testing, and debugging.

### Electronic Engineering Intern — China ACG Group
**July–August 2025**

- Developed **STM32 C/C++ firmware** for sensor interfaces, PWM motor control, and voice-module communication; debugged hardware–firmware behavior through **SWD**.
- Designed a 5 V → 3.3 V power-regulation network with reported efficiency above 85%, and defined a **4-layer PCB** stack-up and decoupling strategy.

### AI Engineer Intern — Sciencia AI
**May–June 2026**

- Built a Python/SQLite ETL workflow using Google Play review data from five apps, with **1,272 cleaned records**.
- Implemented TF-IDF + logistic regression sentiment classification (**80.3% accuracy**) and a Streamlit dashboard.
- Supported component integration, software testing, debugging, and cross-functional development.

## Engineering projects

| Project | Implementation & evaluation | Relevant strengths |
| --- | --- | --- |
| **FPGA VGA Maze Game** — Project Leader, Sept–Dec 2025 | Verilog on Cyclone V; VGA timing, game FSMs, collision detection, PS/2 decoding; ModelSim and on-board testing; 640×480 at 60 FPS; MIF re-encoding reduced memory use by **22%** | Modular RTL, synchronous logic, simulation, FPGA bring-up |
| **Embedded AI Planner** — DE1-SoC | C implementation with a four-state FSM, memory-mapped I/O drivers, and interrupt-driven architecture | Computer organization, register-level interfaces, hardware–software integration |
| **RF Power Amplifier Verification Study** | Eight-point requirements matrix; evaluated a 0.04 W result against a 1–10 W requirement; waveform and switching-loss analysis identified gate parasitic capacitance as the reported failure mechanism | Requirements-based validation, first-principles failure analysis |
| **Reconfigurable Wireless Transceiver** | Mixed-signal circuitry and 4-layer PCB; DDS, LNA, mixer, gain stages; DFM/ERC review across **160+ components** | Interface integration, design review, hardware validation |
| **C++ Command-Driven Circuit Simulator** — Oct–Nov 2025 | Kirchhoff's Current Law and Gauss–Seidel iteration; supported **20+ commands** | C++, numerical algorithms, data structures |
| **Bearing Fault Diagnosis** — APS360, May–Aug 2026 | PyTorch convolutional autoencoder on 128×128 STFT spectrograms; leakage-free file-level split; baseline comparisons; **1.000 AUROC / 1.000 AP** on the held-out CWRU subset; 1,000-iteration bootstrap | Python, disciplined evaluation, signal processing, data-leakage investigation |
| **AI Search & Game Playing** — CSC384 | Sokoban search and Mancala minimax / alpha–beta pruning coursework | Algorithms, search, data structures, terminal-state and depth-limit reasoning |

**Additional team engineering:** Led a five-person RYAM design project (Sept 2023–Apr 2024), narrowing 71 concepts to one prototype using structured evaluation. The prototype passed a 24-hour test; the team ranked in the top 8 of 183 teams.

Bearing-diagnosis scores are specific to the evaluated dataset subset and split.

## Technical toolkit

- **RTL & verification:** SystemVerilog, Verilog, testbenches, functional simulation, ModelSim, waveform analysis, fixed-point/BFP arithmetic, FSMs
- **FPGA & architecture:** Cyclone V, DE1-SoC, Quartus Prime, memory/resource trade-offs, DSP datapaths, computer organization
- **Programming:** Python, C, C++, MATLAB, SQL; Git/GitHub
- **Embedded & hardware:** STM32, MMIO, interrupts/ISR, PWM, sensor interfaces, SWD, Altium Designer, 4-layer PCB, DFM/ERC
- **ML & data:** PyTorch, scikit-learn, SQLite, ETL, Streamlit

## Education & publication

**BASc, Electrical Engineering — University of Toronto**  
Minor in Artificial Intelligence & Robotics · Expected **April 2029** · Dean's Merit Award recipient

Relevant coursework: Digital Systems · Computer Organization · Algorithms & Data Structures · Microelectronic Circuits · Signals & Systems · Control Systems · Applied Deep Learning · Introduction to AI.

**B. Cao, Z. Yang, L. Yu, Y. Zhang**, “Research on the star algorithm for safe path planning,” *IEEE ICCECT 2023*, pp. 105–109. [DOI](https://doi.org/10.1109/ICCECT57938.2023.10141167)

[Explore the engineering portfolio →](https://jillian06.github.io/nvidia-asic-verification-portfolio/)
