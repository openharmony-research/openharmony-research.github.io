---
# Page settings
layout: default
keywords:
comments: false

# Hero section
title: ASPLOS'24 tutorial
description: "Exploring System Research with OpenHarmony OS: A Practical Tutorial"

# Author box
# author:
#     title: About Author
#     title_url: '#'
#     external_url: true
#     description: Author description

# Micro navigation
micro_nav: true

# Page navigation
# page_nav:
#     prev:
#         content: Previous page
#         url: '#'
#     next:
#         content: Next page
#         url: '#'
---

## Introduction

In the swiftly changing world of technology, **mobile operating systems** are advancing towards a more distributed, interconnected, and intelligent framework. This evolution demands the creation of operating systems and hardware architectures that are not only secure but also exhibit peak performance and user-friendly simplicity.
**[OpenHarmony](https://openharmony.cn/)** stands at the forefront of this revolution as a cutting-edge OS.
It enables developers to craft secure, interconnected mobile ecosystems through a synergistic approach of hardware-OS co-design.
**This tutorial offers a comprehensive look into the development of futuristic mobile operating systems and architectural designs, using OpenHarmony as the pivotal platform.**

In this tutorial, our main goal is to facilitate a practical learning journey. We'll embark on a detailed exploration of the OpenHarmony operating system, delving into its core principles and structural design. The tutorial will encompass several key areas: firstly, constructing system security prototypes within the OpenHarmony framework, with an emphasis on integrating Trusted Execution Environments (TEE) like RISC-V Penglai. Secondly, we'll focus on utilizing OpenHarmony's distributed hardware abstraction capabilities to efficiently connect multiple OpenHarmony devices.
Lastly, we will show how OpenHarmony enables top-tier research works like VSync (**ASPLOS'21 Distinguished Paper**) and Penglai (**OSDI'21**).

The tutorial will cover the following key topics:

1. Understanding the evolving landscape of mobile OSes and their security requirements.
2. Familiarizing yourself with the features and architecture of OpenHarmony.
3. Step-by-step guidance on building system security prototypes (TEE, application authority) based on OpenHarmony.
4. Step-by-step guidance on building an interconnected system using the distributed capability based on OpenHarmony (e.g., distributed TEE).
5. Step-by-step guidance on verification and optimization for synchronization primitives based on OpenHarmoy with VSync/LibVSync.
6. Demonstrating how OpenHarmony and related systems facilitate novel ideas and reliable experimentation for researchers and system designers.

This tutorial is designed for researchers, system designers, and developers interested in exploring and harnessing the potential of OpenHarmony to create next-generation mobile OS solutions.



<div class="callout callout--warning">
    <p><strong>Join us (!!!)</strong> In this tutorial to unlock new opportunities and pave the way for secure, interconnected and efficient mobile systems using OpenHarmony. </p>
</div>

## Organizers

<!-- * **Dong Du**, Assistant Professor, Shanghai Jiao Tong University, dd_nirvana@sjtu.edu.cn
* **Jing Zhang**, Master student, Shanghai Jiao Tong University
* **Erhu Feng**, Ph.D student, Shanghai Jiao Tong University
* **Yubin Xia**, Full Professor, Shanghai Jiao Tong University
* **Zeyu Mi**, Associate Professor, Shanghai Jiao Tong University
* **Qingyuan Liu**, Ph.D student, Shanghai Jiao Tong University -->

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/dongdu-2024-1400.webp" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Dong Du</strong>
    <p>Assistant Professor, IPADS Lab, Shanghai Jiao Tong University. Research interests include OS and architecture.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/jing_zhang.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Jing Zhang</strong>
    <p>1st-year master's student, IPADS Lab, Shanghai Jiao Tong University, with a primary research focus on operating systems. I am dedicated to the academic research and development of the open-source project OpenHarmony.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/erhu_feng.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Erhu Feng</strong>
    <p> 4th year Ph.D student, IPADS Lab, Shanghai Jiao Tong University. Research direction is system architecture and security, published papers in OSDI, ASPLOS, ISCA, HPCA. Maintainer of Penglai RISC-V TEE (open-sourced).
</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <!-- <img src="/imgs/xiayubin-new.jpg" alt="Description of Image"> -->
    <img src="/imgs/xiayubin.png" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Yubin Xia</strong>
    <p>Full Professor, IPADS Lab, Shanghai Jiao Tong University. Research interests include operating systems, computer architecture.
</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/zeyumi.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Zeyu Mi</strong>
    <p>Associate professor at School of Software, IPADS Lab, Shanghai Jiao Tong University. Research interests include AIGC (LLM) systems, OS, system virtualization, and system security. Leader of PowerInfer framework (open-sourced).
</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/qingyuan_liu.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Qingyuan Liu</strong>
    <p>3rd-year Ph.D student, IPADS Lab, Shanghai Jiao Tong University. Advisor: Haibo Chen, Yubin Xia, and Dong Du. Research areas are serverless computing and cloud-native systems.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/diogo-behrens-602fbb95.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Diogo Behrens</strong>
    <p>Behrens is research engineer at HW Dresden Research Center, currently leading the System Software Concurrency team. Before joining HW in 2019, Diogo was software engineer with focus on stream data processing. He holds a PhD from TU Dresden, Germany.</p>
  </div>
</div>

## Agenda

**Date: Saturday, April 27th, Afternoon**

**Location: Hilton La Jolla Torrey Pines, San Diego, California (with ASPLOS'24)**

### Prerequisite

- **Prior knowledge of operating systems and basic programming concepts would be beneficial.**

- **Please bring a laptop, that can allow you do some experiments :)**

- **Devices: we will provide simulator for OpenHarmony, and cloud servers that you can connect for most experiments. We will also bring some dev-boards that allow you to try the OS on real devices.**

### Contents and Timeline

The planed topics and timeline are the following:

| Time   | Topic                                                        | Speaker              | Slides | Code |
|:-------|:-------------------------------------------------------------|:---------------------|:-----------:|:------:|
| **1:40pm** | Part 1: Introduction to OpenHarmony *(20min)*             | Yubin Xia            |             |        |
| **2:00pm** | Exercise 1: How to build OpenHarmony & Toolchains for OpenHarmony<br />*(20min)* | All |             | [code](https://github.com/openharmony-research/helloworld-demo) |
| **2:20pm** | Part 2: Distributed functionality of OpenHarmony *(20min)*  | Dong Du              |             |        |
| **2:50pm** | Coffee Break *(20min～30min)*                                | \ | \ | \ |
| **3:20pm** | Exercise 2: Distributed Capability of OpenHarmony *(20min)* | Jing Zhang & <br />Qingyuan Liu |       | [code](https://github.com/openharmony-research/distributedcalc-demo) |
| **3:40pm** | Part 3 & Exercise3: Concurrency Research based on OpenHarmony *(40min)* | Diogo Behrens| [slides](https://github.com/open-s4c/demo-asplos24) | [code](https://github.com/open-s4c/demo-asplos24) |
| **4:20pm** | Part 4: Security Research based on OpenHarmony *(20min)*                   | Erhu Feng            |             |        |
| **4:40pm** | Exercise 4: Penglai TEE Demo                          | All                  |             |        |
| **4:55pm** | Research Opportunities & Outlook (Conclusion & Remark )      | Yubin Xia            |             |        |
| **5:00pm** | Q/A                                                          | All                  |             |        |

## Credits

We thank the following people/organizations for their huge supports for the 1st OpenHarmony Research Tutorial (in no particular order).

* OpenHarmony TSC.
* Jiageng Yu (于佳耕, ISCAS) and Yang Tai (邰阳, ISCAS) help on the OpenHarmony Simulator (based on their PolyOS project) that is used for demos/experiments.
* Ming Fu gives suggestions on the content of this tutorial.
* Yutao Liu gives suggestions on the content of this tutorial.
* Guo Liu (刘果)
* and Others
