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

In the swiftly changing world of technology, mobile operating systems are advancing towards a more distributed, interconnected, and intelligent framework. This evolution demands the creation of operating systems and hardware architectures that are not only secure but also exhibit peak performance and user-friendly simplicity. OpenHarmony (https://openharmony.cn/) stands at the forefront of this revolution as a cutting-edge operating system. It enables developers to craft secure, interconnected mobile ecosystems through a synergistic approach of hardware-OS co-design. This tutorial offers a comprehensive look into the development of futuristic mobile operating systems and architectural designs, using OpenHarmony as the pivotal platform.

In this tutorial, our main goal is to facilitate a practical learning journey. We'll embark on a detailed exploration of the OpenHarmony operating system, delving into its core principles and structural design. The tutorial will encompass several key areas: firstly, constructing system security prototypes within the OpenHarmony framework, with an emphasis on integrating Trusted Execution Environments (TEE) like RISC-V Penglai. Secondly, we'll focus on utilizing OpenHarmony's distributed hardware abstraction capabilities to efficiently connect multiple OpenHarmony devices. Lastly, we will cover the "develop once, run anywhere" paradigm, emphasizing the cross-platform compatibility of OpenHarmony.

The tutorial will cover the following key topics:

1. Understanding the evolving landscape of mobile operating systems and their security requirements.
2. Familiarizing yourself with the features and architecture of OpenHarmony.
3. Step-by-step guidance on building system security prototypes (TEE, application authority) based on OpenHarmony.
4. Step-by-step guidance on building an interconnected system using the distributed capability based on OpenHarmony (e.g., distributed TEE).
5. Step-by-step guidance on how to develop OpenHarmony applications once but run on different platforms
6. Demonstrating how OpenHarmony and related systems facilitate novel ideas and reliable experimentation for researchers and system designers.

This tutorial is designed for researchers, system designers, and developers interested in exploring and harnessing the potential of OpenHarmony to create next-generation mobile OS solutions. Prior knowledge of operating systems and basic programming concepts would be beneficial.


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
    <p>I am an Assistant Professor in the Institute of parallel and distributed systems (IPADS), Shanghai Jiao Tong University. My research interests include operating systems, architecture, system security (TEE), serverless computing and HW/SW co-design. I have built several systems including Penglai TEE (state-of-the-art RISC-V TEE), serverless systems (Catalyzer, ServerlessBench, and Molecule), and RISC-V IPC extension (XPC). I am also working on open-sourced communities, including RISC-V (SPMP TG chair), openEuler (RISC-V SIG maintainer) and OpenHarmony (RISC-V and TEE SIG maintainer).</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/jing_zhang.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Jing Zhang</strong>
    <p>I am a first-year master's student at the Institute of Parallel and Distributed Systems, Shanghai Jiao Tong University, with a primary research focus on operating systems. I am dedicated to the academic research and development of the open-source project OpenHarmony.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/erhu_feng.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Erhu Feng</strong>
    <p> Institute of Parallel and Distributed Systems, Shanghai Jiaotong University, fourth year PhD student, main research direction is system architecture and security, published many academic papers in OSDI, HPCA and other international conferences and journals, participated in China's first open source enclave project (Penglai), and at the same time, committed to open source development as well as product landing.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <!-- <img src="/imgs/xiayubin-new.jpg" alt="Description of Image"> -->
    <img src="/imgs/xiayubin.png" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Yubin Xia</strong>
    <p>I am a professor in School of Software at Shanghai Jiao Tong University and a member of Institute of Parallel And Distributed Systems (IPADS). My research interests include operating systems, computer architecture. Currently, I'm now focusing on hardware-software co-design for better performance and isolation. Some recent projects by my students and colleagues include the Penglai (蓬莱) RISC-V TEE, the XPC architecture extension for fast IPC, the Catalyzer serverless framework with &lt; 1ms startup latency, the ServerlessBench test suit for serverless frameworks, and the DeSearch search engine for web3.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/zeyumi.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Zeyu Mi</strong>
    <p>I am an associate professor at School of Software, Shanghai Jiao Tong University (SJTU). I obtained my Ph.D. in computer science from SJTU, advised by Prof. Haibo Chen and Prof. Binyu Zang. My research interests include AIGC systems, operating systems, system virtualization, and system security. I obtained my bachelor degree in software engineering from Nanjing University in 2014.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/qingyuan_liu.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Qingyuan Liu</strong>
    <p>I am a third-year doctoral candidate at the Institute of Parallel and Distributed Systems, Shanghai Jiao Tong University. Under the guidance of Professors Chen Haibo, Xia Yubin, and Du Dong, my current main research areas are operating systems, virtualization, and cloud computing.</p>
  </div>
</div>

## Agenda

**Date: Saturday, April 27th, Afternoon**

**Location: Hilton La Jolla Torrey Pines, San Diego, California (with ASPLOS'24)**


| Time   | Topic                                                        | Speaker              | Slides | Code |
|--------|--------------------------------------------------------------|----------------------|-------------|--------|
| **1:40pm** | Part 1: Introduction to OpenHarmonyOS (20min)               | Yubin Xia            |             |        |
| **2:00pm** | Exercise 1: How to build OpenHarmony & Toolchains for OpenHarmony (20min) | All |             |        |
| **2:20pm** | Part 2: Distributed functionality of OpenHarmony (20min)    | Dong Du              |             |        |
| **2:50pm** | Coffee Break (20min～30min)                                  | \ | \ | \ |
| **3:20pm** | Exercise 2: Distributed Capability of OpenHarmony OS (20min) | Jing Zhang & Qingyuan Liu |       |        |
| **3:40pm** | Part 3: Declarative Application Development /OH Concurrency Research (20min) | Diogo |             |        |
| **4:00pm** | Exercise 3: Declarative UI and App Development demo VSync/LibVSync Demo on OH (20min) | Diogo | |        |
| **4:20pm** | Part 4: Security in OpenHarmony (20min)                     | Erhu Feng            |             |        |
| **4:40pm** | Exercise 4: Security demo (Penglai)                          | All                  |             |        |
| **4:55pm** | Conclusion & Remark (Research opportunities & outlook)      | Yubin Xia            |             |        |
| **5:00pm** | Q/A                                                          | All                  |             |        |

## Credits

We thanks the following people/organizations for their huge supports for the 1st OpenHarmony Research Tutorial (in no particular order).

* OpenHarmony TSC.
* Jiageng Yu (于佳耘, ISCAS) and Yang Tai (邰阳, ISCAS) help on the OpenHarmony Simulator (based on their PolyOS project) that is used for demos/experiments.
* Ming Fu gives suggestions on the content of this tutorial.
* Yutao Liu gives suggestions on the content of this tutorial.
* Guo Liu (刘果)
