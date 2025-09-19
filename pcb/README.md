# this pcb is currently under active development!
currently designing power supplies

## schematic hierarchy structure
```
├── RPi-HwAB-1.kicad_sch                 # top-level schematic
│   └── main-pwr.kicad_sch               # quad-buck converter for fpga, I-sense networks
│   │	 └── compensation.kicad_sch      # bulk decoupling and compensation networks for adp5054
│   └── fpga.kicad_sch                   # artix-7 35t abstraction
│   │    └── fpga-pwr.kicad_sch          # fpga power pins
│   │    │    └── decoupling.kicad_sch   # decoupling for fpga power rails
│   │    └── fpga-1.kicad_sch            # jtag, bank 14, bank 15
│   │    └── fpga-2.kicad_sch            # banks 16, 34, 35
│   │    └── fpga-3.kicad_sch            # mgt bank (216)
│   │    └── memory.kicad_sch            # spi flash / eeprom
│   └── sensors.kicad_sch                # temperature and current sensors
│   └── connectors.kicad_sch             # pcie, gpio, and jtag connectors
```


power requirements:

adp5054: 5V

misc. sensors: 3.3V

FPGA:
  1. vccint, vccbram, mgtavcc: 1.0V
  2. vccaux: 1.8V
  3. mgtavtt: 1.2V
  4. vcco: probably lvcmos 3.3V

### top-level schematic as of september 19, 2025
<img width="3507" height="2480" alt="image" src="https://github.com/user-attachments/assets/f98d1b37-bfdc-45bd-a397-b0e95f8326af" />
