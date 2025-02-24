---
# Page settings
layout: default
keywords:
comments: false

# Hero section
title: ASPLOS'25 tutorial
description: "OpenHarmony OS in System Research: A Practical Guide"

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
OpenHarmony is a rapidly expanding open-source operating system. With its deployment on over 100 million commercial devices, it has emerged as one of the most popular open-source OS platforms in the mobile industry. It offers a wealth of research possibilities by enabling more seamless integration and co-design between the operating system and its underlying hardware architecture.
This tutorial is designed as a hands-on learning journey into OpenHarmony. We'll embark on a detailed exploration of the OpenHarmony operating system, delving into its core principles and structural design. The tutorial will encompass several key areas:

* **Introduction to OpenHarmony Architecture:** we’ll begin with an overview of the evolving mobile OS landscape, emphasizing the unique features and architecture of OpenHarmony.
* **Practical Development and Prototyping:** step-by-step instructions will guide you through building system security prototypes, utilizing underlying synchronization primitives, and designing scalable data structures. Additionally, we’ll cover the experience of porting existing applications to OpenHarmony.
* **Innovative Experimentation and System Research:** finally, we’ll demonstrate how OpenHarmony enables novel research ideas and supports reliable experimentation for researchers and system designers.
By the end, participants will have gained a comprehensive, practical understanding of OpenHarmony’s potential in system research and development.

The tutorial will cover the following key topics:

1. Understanding the evolving landscape of mobile operating systems, elaborating the features and architecture of OpenHarmony.
2. Step-by-step guidance on building system security prototypes (TEE, application authority) based on OpenHarmony.
3. Step-by-step guidance on building an scalable concurrent data structure in OpenHarmony with formal methods
4. Step-by-step guidance on how to develop OpenHarmony applications, as well as how to port existing applications into OpenHarmony
5. Demonstrating how OpenHarmony enables novel research ideas and supports reliable experimentation for researchers and system designers.


<div class="callout callout--warning">
    <p><strong>Join us (!!!)</strong>In this tutorial to unlock new opportunities and pave the way for secure, interconnected and efficient mobile systems using OpenHarmony. Prior knowledge of operating systems and basic programming concepts would be beneficial.</p>
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
    <img src="/imgs/liuyutao.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Yutao Liu</strong>
    <p>Director of Huawei Dresden Research Center. He received his PhD from Shanghai Jiao Tong University in 2017. Research interests include OS and architecture.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/diogo-behrens.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Diogo Behrens</strong>
    <p>Behrens is the director of Dresden OS Kernel Lab at HW Dresden Research Center. Before joining HW in 2019, Diogo was software engineer with focus on stream data processing. He holds a PhD from TU Dresden, Germany.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/lixinrui.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Xinrui Li</strong>
    <p>5th year Ph.D. student, IPADS Lab, Shanghai Jiao Tong University. Research focuses on performance optimization in mobile OS. Serve as a teaching assistant for the Computer System Design and Implementation (Using OpenHarmony) course at Shanghai Jiao Tong University.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/magnus-morton.png" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Magnus Morton</strong>
    <p>Magnus Morton is an expert in the Programming Languages lab at the Huawei Edinburgh Research Centre, specializing in the research and application of Effect Handlers technology in the Cangjie Programming language.</p>
</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/francesco-pham.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Francesco Pham</strong>
    <p></p>
</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/jonathan-schwender.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Jonathan Schwender</strong>
    <p></p>
</p>
  </div>
</div>

## Agenda

**Date: Monday, March 31th, Morning**

**Location: Room Goudriaan I, Postillion Hotel & Convention Centre WTC Rotterdam, Beursplein 37, 3011 AA Rotterdam, The Netherlands. (with ASPLOS & EuroSys 2025)**

### Prerequisite

- **Prior knowledge of operating systems and basic programming concepts would be beneficial.**
- **Please bring a laptop, that can allow you do some experiments :)**
- **Please install some necessary apps in your laptop:**
  1. **VNC client**: we need to connect up to 2 VNC servers, [realVNC](https://www.realvnc.com/en/) is recommended
  2. **7z**: we use 7z to decompress pre-compiled images. Download in [official website](https://www.7-zip.org/download.html) is enough
  3. **DevEco Studio IDE**: If you want to experience the entire process of compiling an OpenHarmony application, please refer to the slides for Exercise 1 and install DevEco Studio before the tutorial
- **Devices: we will provide simulator for OpenHarmony, and cloud servers that you can connect for most experiments. We will also bring some dev-boards that allow you to try the OS on real devices.**

### Contents and Timeline

The planed topics and timeline are the following:

| Time   | Topic                                                        | Speaker              | Slides | Code |
|:-------|:-------------------------------------------------------------|:---------------------|:-----------:|:------:|
| **9:00am** | Part 1: Introduction to OpenHarmony *(10min)* | Yutao Liu | [slides]() | |
| **9:10am** | Exercise 1: How to build OpenHarmony & Toolchains for OpenHarmony *(20min)* | Jonathan Schwender | [slides]() | [code]() |
| **9:30am** | Part 2 & Exercise 2: OpenHarmony Application Development 101 *(30min)* | Xinrui Li | [slides]() | [code]() |
| **10:00am** | Part 3 & Exercise 3: Concurrency Research based on OpenHarmony *(30min)* | Diogo Behrens | [slides]() | [code]() |
| **10:30am** | Coffee Break *(30min)* | All | \ | \ |
| **11:00am** | Part 4 & Exercise 4: Cangjie for OpenHarmony Native Application Development *(30min)* | Magnus Morton | [slides]() | [code]() |
| **11:30am** | Part 5 & Exercise 5: Oniro Introduction and Development Guide *(30min)* | Francesco Pham | [slides]() | [code]() |
| **12:00am** | Research Opportunities & Outlook (Conclusion & Remark) *(10min)* | Yutao Liu | | |
| **5:00pm** | Q/A *(10min)* | All | | |

## Topics Introduction

| **Part 1: Introduction to OpenHarmony** <br />Intro |
| **Part 2: OpenHarmony Application Development 101**<br /> This session provides a hands-on introduction to OpenHarmony application development. Through a practical example, we will explore key aspects of OpenHarmony development, including declarative UI design with ArkTs, utilization of system capabilities such as audio, and multi-device collaboration. |
| **Part 3: Concurrency Research based on OpenHarmony**<br />Intro |
| **Part 4: Cangjie for OpenHarmony Native Application Development**<br />Cangjie is a new, general-purpose programming language developed by Huawei, designed to improve performance and developer productivity. It is intended for a wide range of scenarios, from servers to OpenHarmony mobile phones. In this tutorial, we will present an introduction to the Cangjie Programming language, explaining the basics of  its syntax and semantics, before looking at how Cangjie can be used to build rich OpenHarmony applications. The second part of the tutorial will explore Cangjie's Effect Handlers. Effect handlers are and advanced construct for custom concurrency and programmable control flow. We will show how to use this feature, along with some details of the implementation. We will then look at some more complex and practical uses of Effect Handlers in the OpenHarmony ecosystem, demonstrating the power and flexibility of the feature. |
| **Part 5: Oniro Introduction and Development Guide**<br />Intro |

## Credits

We thank the following people/organizations for their huge supports for the 1st OpenHarmony Research Tutorial (in no particular order).

* OpenHarmony TSC.
* Ming Fu gives suggestions on the content of this tutorial.
* Yubin Xia gives suggestions on the content of this tutorial.
* Dong Du gives suggestions on the content of this tutorial.
* Jiang Rui gives suggestions on the content of this tutorial.
* Guo Liu (刘果)
* and Others
