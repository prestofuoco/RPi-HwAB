## schematic hierarchy structure
```
├── RPi-HwAB-1.kicad_sch                 # top-level schematic
│   └── main-pwr.kicad_sch               # quad-buck converter for fpga, I-sense networks
│   │	 └── sequencing.kicad_sch        # power sequencing for adp5054
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

### top-level schematic as of november 4, 2025
<img width="3507" height="2480" alt="image" src="https://github.com/user-attachments/assets/1c64b538-1f11-4ff5-89eb-b3a78b70efe6" />
