LAN8720 board for MangoPi MQ-Pro
================================

In the first iteration I tested the experimental patch based on `arch/riscv/boot/dts/allwinner/sun20i-d1-nezha.dts` rather than `arch/riscv/boot/dts/allwinner/sun20i-d1-mangopi-mq-pro.dts` with bread-board version of the schematic.

The patch and the table of connections is added. It will be moved to the legacy secion once I have the v1 schematics, board and final DT.

License
-------

TBD: This will be open source/OpenHW for sure.

dmesg output
------------

```
[  104.125393] dwmac-sun8i 4500000.ethernet: IRQ eth_wake_irq not found
[  104.125445] dwmac-sun8i 4500000.ethernet: IRQ eth_lpi not found
[  104.126653] dwmac-sun8i 4500000.ethernet: PTP uses main clock
[  104.126754] dwmac-sun8i 4500000.ethernet: Current syscon value is not the default 50006 (expect 0)
[  104.140716] dwmac-sun8i 4500000.ethernet: No HW DMA feature register supported
[  104.140764] dwmac-sun8i 4500000.ethernet: RX Checksum Offload Engine supported
[  104.140794] dwmac-sun8i 4500000.ethernet: COE Type 2
[  104.140826] dwmac-sun8i 4500000.ethernet: TX Checksum insertion supported
[  104.140857] dwmac-sun8i 4500000.ethernet: Normal descriptors
[  104.140885] dwmac-sun8i 4500000.ethernet: Chain mode enabled
[  108.505636] dwmac-sun8i 4500000.ethernet end0: renamed from eth0
[  111.253079] dwmac-sun8i 4500000.ethernet end0: PHY [stmmac-0:01] driver [SMSC LAN8710/LAN8720] (irq=POLL)
[  111.260378] dwmac-sun8i 4500000.ethernet end0: Register MEM_TYPE_PAGE_POOL RxQ-0
[  111.264987] dwmac-sun8i 4500000.ethernet end0: No Safety Features support found
[  111.265046] dwmac-sun8i 4500000.ethernet end0: No MAC Management Counters available
[  111.265085] dwmac-sun8i 4500000.ethernet end0: PTP not supported by HW
[  111.282125] dwmac-sun8i 4500000.ethernet end0: configuring for phy/rmii link mode
[  287.401778] dwmac-sun8i 4500000.ethernet end0: Link is Up - 100Mbps/Full - flow control rx/tx
```
