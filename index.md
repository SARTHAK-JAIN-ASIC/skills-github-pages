---
layout: default
title: Sarthak Jain - Hardware Engineering Portfolio
---

<link rel="stylesheet" href="/skills-github-pages/custom.css">

<style>
/* Light/Dark Mode Toggle */
body.light-mode {
  background-color: #ffffff;
  color: #000000;
}
body.dark-mode {
  background-color: #0f0f0f;
  color: #f0f0f0;
}
.toggle-container {
  position: fixed;
  top: 1rem;
  right: 1rem;
}
.toggle-container label {
  cursor: pointer;
  font-size: 0.9rem;
}
</style>

<div class="toggle-container">
  <label>
    <input type="checkbox" id="modeToggle"> Toggle Dark Mode
  </label>
</div>

<script>
  const toggle = document.getElementById('modeToggle');
  toggle.addEventListener('change', function() {
    document.body.classList.toggle('dark-mode');
    document.body.classList.toggle('light-mode');
  });
  document.body.classList.add('light-mode');
</script>

# 👋 Hey there! I'm Sarthak

Welcome to my portfolio! I’m a Master’s student in **Electrical Engineering, specializing in Computer Architecture** at **USC**, blending academic depth with **4+ years of hands-on work experience** in **ASIC/FPGA design**, **RTL development**, and **hardware acceleration** and **verification**.

I've had the privilege of working on **cutting-edge hardware systems** across both early-stage and startup-mode teams—at **Marquee Semiconductor**, where I optimized compute-heavy architectures, and **Baker Hughes**, where I developed fault-tolerant systems for industrial-grade deployments. Whether it’s building a **custom out-of-order CPU**, integrating **PCIe and DDR subsystems**, or scaling AI accelerators on **NetFPGAs**, I take pride in delivering **high-performance, timing-closed** hardware.

---

## What Drives Me

I thrive at the intersection of architecture and implementation, **designing, debugging, and optimizing** systems from RTL to silicon. I love taking ownership across the stack, from **schematic design and validation**, to **hardware-software co-design**, **chip multiprocessor modeling**, and **GPGPU architecture simulation**.

> “I enjoy building things from scratch, whether it’s a Tomasulo-based CPU, a DMA-backed packet classifier, or a UVM-based verification testbench that breaks the system before production does.”

---

## Tech Stack & Interests

- **Languages:** Verilog, SystemVerilog, C++, Python, TCL, VHDL  
- **Verification & Tools:** UVM, Vivado, Vitis, Synopsys VCS, QuestaSim, ModelSim, Cadence Virtuoso, ChipScope  
- **Simulation & Research:** GEM5, GPGPU-Sim, NetFPGA  
- **Protocols:** PCIe, AXI, AHB/APB, UART, SPI, I2C  
- **Concepts:** Out-of-order execution, Tomasulo’s algorithm, cache coherence (MOESI/MESIF), branch prediction, pipelining, memory systems, multicore design, async/sync FIFOs, DRAM architecture, DDR, CAM-based caching, Static Timing Analysis  

---

## What I’m Studying at USC

Courses like **Advanced Computer Architecture**, **Network Processor Design**, and **Digital System Microarchitecture** are sharpening my edge in scalable computing and real-world systems design. I currently work as a **research assistant** on **AI-accelerated SmartNICs**.

---

## Featured Projects

-  [Tomasulo Out-of-Order CPU (GitHub)](https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/OoO_CPU_Tomasulo)
-  [4-core, 16-thread CMP (GitHub)](https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/Chip_Multiprocessor_4Core_16Thread)
-  [PCIe PHY Implementation (PPT)](https://github.com/SARTHAK-JAIN-ASIC/EE533/blob/main/PCIe_PHY_Project/PCIe_PHY_SarthakJain.pdf)
-  [AI-Based Packet Classifier on SmartNIC (GitHub)](https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/AI_based_Network_Classification_NPU_Project/final_v6)
-  [ARMv7 Pipelined CPU with CAM Cache (PPT)](https://github.com/SARTHAK-JAIN-ASIC/EE533/blob/main/ARMv7_CPU_with_CAM_Cache/Presentation_ARMv7_Sarthak.pdf)
-  [Async FIFO with Burst Buffer (GitHub)](https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/Async_FIFO_with_LowLatencyBurstBuffer)

---

## 📅 Timeline

**Research Assistant – USC (Mar 2025 – May 2025)**  
Built a full hardware-software integrated SmartNIC with DMA-enabled NPU for real-time packet classification (2.2 Gbps throughput, 12× faster than baseline).

**RTL/FPGA Design Engineer – Baker Hughes (Jun 2021 – Jul 2024)**  
Designed fault-tolerant packet parsing engines on Zynq MPSoC, built full SystemVerilog testbench environment, reduced time-to-market by 30%.

**Digital Design Engineer – Marquee Semiconductor (Sep 2019 – Jun 2021)**  
Built systolic arrays, reduced power by 23%, and deployed high-speed kernels with OpenCL on AMD accelerators (U250/U50).

---

## Let's Connect

-  [LinkedIn](https://www.linkedin.com/in/sarthak-jain-ms-ee/)
-  [GitHub](https://github.com/SARTHAK-JAIN-ASIC)
-  Email: sarthakj84@gmail.com or sarthakj@usc.edu
-  [Project Playlist (YouTube)](https://youtube.com/playlist?list=PLLlDYTD17uuSVnh_l-IZ8kwdkERV3T-qU&si=0SrZ2BsS0m5h0ENy)

---

Thanks for visiting! Scroll up to explore, or feel free to reach out if you’re building something impactful in silicon or systems design.
