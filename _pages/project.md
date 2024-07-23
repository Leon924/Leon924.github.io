---
title: "Project"
permalink: /project/
author_profile: true
---

## Lightweight Power Modeling for Complex Power Patterns in Heterogeneous Platforms
<!-- 2023.1-2024.4 -->

- Feature selection algorithm for bit-level power proxies: Efficiently extracts tens to hundreds of proxies from millions of RTL bits: only requires 0.028% of NVDLA (NVIDIA) RTL bits and 0.036% of BOOM (UC Berkeley) RTL bits, significantly reducing the input processing and inference burden of power prediction models on chip.
- Lightweight high-precision power prediction algorithm: designed an efficient power prediction algorithm. The cycle-by-cycle power prediction error on BOOM and NVDLA is reduced to 2.49% and 1.69% respectively. In power peak prediction, the error of more than 95.5% of the samples is lower than 5%, surpassing SOTAs' performance.
- Multi-objective optimization framework for coordinating software and hardware metrics: Designed a multi-objective optimization framework for the on-chip power meter (OPM) focusing on the dual objectives of accuracy and on-chip overhead, which efficiently searched 52 Pareto front solutions from 8192 experiments within 3.5 hours.
- High-throughput low-overhead on-chip power meter design: Implemented the proposed power prediction algorithm as an OPM. The area and power overhead of the NVDLA OPM are 0.49% and 0.097%, respectively. The cycle-by-cycle prediction delay is only 3 cycles, providing nanosecond-level power monitoring capability (under T28 process).
  
## Low-Power High-Sensitivity Gesture Recognition Chip Design（National Key Research and Development Program of China）
<!-- 2019.12 - 2022.10 -->
- Architecture and Frontend: Designed and implemented a SoC architecture based on the Rocket Core and developed the RoCC coprocessor with custom extension instructions to support real-time, high-precision dynamic gesture recognition, achieving an accuracy of 93%-99%. (assitant)
- Prototype Verification: Established a prototype verification platform using the Arty-A7 development board and the CMOS image sensor OV5640. Completed functional verification of the coprocessor and SoC architecture. (assitant)
- Tape-out and Testing: Completed the mid- and backend flow of the chip using TSMC 28nm process. Implemented various low-power techniques including multiple clock domains, clock gating, multiple voltage domains, and memory sleep control. The chip can achieve 30FPS dynamic gesture recognition with a power consumption of 397µW@0.584V, and its standby power at room temperature is only 78.3µW. (Responsible)


## Design Space Exploration of RISC-V Core Microarchitecture
<!-- 2021.10-2022.12 -->
- Sampling Algorithm Design: designed a hybrid sampling algorithm that integrates edge design points and central proximity design points. This algorithm efficiently completes optimization within a subspace of 1024 with only 7 initial samples, demonstrating low preparation effort.
- Multi-Objective Bayesian Optimization Algorithm Design: Developed a parallel DKL-GP algorithm as a surrogate model. Used the EHVI of the tri-objective hypervolume in the objective space as the acquisition function. The BO algorithm can find the optimal solution in just 6 iterations with parallel of 3, showing high time efficiency.
- Automated End-to-End Microarchitecture Simulation Platform Design: Designed and implemented the SPA-Gen simulation platform to parallelly obtain performance responses for multiple elite samples and automatically output the SPA of elite samples, ensuring a fully automated VLSI process.

<!-- 所提出的设计空间探索（DSE）技术在UC Berkeley BOOM 处理器内核上完成了实验验证。相关工作发表在领域高水平期刊 
Microelectronic Journal（MJ） \\\textit{https://www.sciencedirect.com/science/article/abs/pii/S0026269222003081}（第一作者） -->