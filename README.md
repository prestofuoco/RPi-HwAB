# raspberry pi 5 hardware acceleration hat+ with xc7a

> **⚠️ work in progress:** this project is currently in the active pcb design and development phase. the hardware is not yet finalized or available. the repository structure, code, and documentation are placeholders for what is planned. stay tuned for updates!

## overview

welcome to the official repository for my raspberry pi 5 hat+ hardware accelerator. this project aims to create a powerful accelerator board featuring a xilinx artix-7 (xc7a) fpga. the goal is to bring high-speed, parallel processing capabilities to the raspberry pi 5, enabling a new generation of projects in fields like real-time signal processing, machine learning, and computer vision.

currently, the focus is on the **pcb design and layout**. the `pcb/` directory contains the most up-to-date work. other sections of this repository, such as `fpga_src` and `examples`, contain planned structures and will be developed once the hardware is stable.

## planned key features

* **xilinx artix-7 fpga:** will utilize the powerful and efficient xc7a series fpga for custom hardware acceleration
* **hat+ compliant:** designed to the latest raspberry pi hat+ specification for seamless integration and configuration
* **high-speed pcie interface:** aims to leverage the raspberry pi 5's pcie capabilities for maximum data throughput
* **on-board peripherals:** the design will include various peripherals which will be noted here
* **open-source design:** the pcb design, verilog/vhdl examples, and host software will be open-source and available in this repository

## hardware and software requirements (provisional)

### hardware

* a raspberry pi 5
* the final version of this xc7a fpga hat+ board
* a reliable power supply for the raspberry pi 5 (5v/5a recommended)

### software (provisional)

* **raspberry pi os:** ubuntu server 20.04+
* **xilinx vivado design suite:** for developing fpga bitstreams
* **kicad:** for viewing and editing the pcb design files

## project status

this project is currently focused on hardware development.

### 1. pcb design

the kicad project files can be found in the `pcb/` directory. this is the primary area of development right now. feedback and contributions for schematics and layout are welcome.

### 2. future steps (post-hardware)

once the pcb is finalized and fabricated, development will shift to:

1. **board bring-up and testing:** verifying all hardware components.
2. **fpga development:** creating example bitstreams (e.g., led blinker, pcie communication).
3. **host-side software:** writing drivers and libraries to communicate with the fpga from the raspberry pi.

## repository structure

```
.
├── bitstreams/       # (planned) pre-compiled fpga bitstream files
├── docs/             # (planned) detailed documentation and datasheets
├── examples/         # (planned) example projects (host-side code)
├── fpga_src/         # (backlog) verilog/vhdl source code for the fpga
│   └── RPi-HwAB-1/   # main vivado project files
│   └── test/         # pinout verification/experimentation
├── pcb/              # (active development) kicad/altium project files
│   └── simulations/  # ltspice simulation files
├── scripts/          # (planned) installation and helper scripts
├── utils/            # (planned) host-side utility programs
└── readme.md         # this file
```

## contact

andre winkel 14 [at] gmail [dot] com

andre [dot] winkel [at] email [dot] ucr [dot] edu

project link: [https://github.com/prestofuoco/rpi-hwab](https://github.com/prestofuoco/rpi-hwab)
