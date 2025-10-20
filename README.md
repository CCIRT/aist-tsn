# AIST-TSN

AIST-TSN is an open source project developed by the National Institute of Advanced Industrial Science and Technology (AIST), Japan. It focuses on enabling hardware design support for Time Sensitive Network (TSN) technology. 
TSN is a set of IEEE standards that extends Ethernet to support real-time, deterministic communication — essential for applications in industrial automation, automotive systems, and cyber-physical infrastructure.
This repository provides design assets, reference implementations, verification tools, and evaluation experiments for TSN features targeting FPGA or ASIC-based hardware development. 
The project aims to accelerate TSN adoption by offering reusable, standards-aligned components and resources for developers, researchers, and system integrators.
We aim to provide an open platform that can be used as a reference design so scientists can implement their desired functionalities and make the different evaluations and comparisons to highlight the appropriate design choices for a given TSN system.

## Design
### AIST TSN Switch
[This repository](https://github.com/CCIRT/aist-tsn-switch) introduces the hardware design of a reconfigurable architecture of an FPGA-based an L2 network switch supporting Time Sensitive Network (TSN). 
It supports two different scheduling algorithms which are implemented and validated on an AMD Xilinx KC705 FPGA evaluation board and a Digilent Zedboard FPGA development board.

- L2 switch supporting Credit Based Shaper (CBS):
- L2 switch supporting Asynchronous Traffic Shaper (ATS)

### AIST EFCC
[This repository](https://github.com/CCIRT/aist-tsn-efcc) includes Ethernet Frame Crafter & Capture (EFCC), a flexible FPGA-based frame generation and capture measurement tool for TSN research and developement. 
EFCC is capable of generating multiple TSN flows with different characteristics, where the frame size, frame rate, and burst size are independently set for each flow. 
In addition, it can record the arrival times of all the frames with a high-precision hardware clock without any loss of the arrival time records, even with the shortest frame size.
EFFC is implemented and validated on an AMD Xilinx KC705 FPGA evaluation board.


## Publications

When using the provided designs in this repository, please refer to the following citations:

AIST TSN Switch for Credit-based Shaper (CBS):
> Akram BEN AHMED, Takahiro HIROFUCHI, and Takaaki FUKAI "FPGA-based Network Switch Architecture Supporting Credit Based Shaper for Time Sensitive Networks", The 29th IEEE International Conference on Emerging Technologies and Factory Automation (ETFA2024), pp. 1-8, Sep 2024, 10.1109/ETFA61755.2024.10710853, https://ieeexplore.ieee.org/document/10710853

AIST TSN Switch for Asynchronous Traffic Shaper (ATS):
> Akram BEN AHMED, Takahiro HIROFUCHI, and Takaaki FUKAI, "Hardware design and Evaluation of an FPGA-based Network Switch Supporting Asynchronous Traffic Shaping for Time Sensitive Networking", IEEE Access, vol. 12, pp. 123149-123165, Aug 2024, doi: 10.1109/ACCESS.2024.3451448, https://ieeexplore.ieee.org/document/10658978

AIST Ethernet Frame Crafter & Capture (EFCC):
> Akram BEN AHMED, Takahiro HIROFUCHI, and Takaaki FUKAI, "EFCC: Ethernet Frame Crafter & Capture for TSN Research", The 50th IEEE Conference on Local Computer Networks (LCN2025), pp. 1-9, October 2025, doi: 10.1109/LCN65610.2025.11146312, https://ieeexplore.ieee.org/document/11146312
> 
> Best Paper Award Candidate🏆


## Contact

The Continuum Computing Architecture Research Group (CCARG), the Intelligent Platforms Research Institute, the National Institute of Advanced Industrial Science and Technology (AIST), Japan.

E-mail: <M-digiarc-ccirt-contact-ml@aist.go.jp>

We are hiring postdocs and technical staffs. Collaborations are also welcome.

## Acknowledgment

This program is based on results obtained from the project, "Research and
Development Project of the Enhanced infrastructures for Post 5G Information and
Communication Systems" (JPNP20017), commissioned by the New Energy and
Industrial Technology Development Organization (NEDO).


## Licensing

Copyright (c) 2024-2025 National Institute of Advanced Industrial Science and Technology (AIST)
All rights reserved.

This software is released under the [MIT License](LICENSE).
