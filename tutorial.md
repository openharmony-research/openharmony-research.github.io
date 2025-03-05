---
# Page settings
layout: default
keywords:
comments: false

# Hero section
title: ASPLOS'25/EuroSys'25 Tutorial
description: "OpenHarmony OS in System Research: A Practical Guide"

micro_nav: true

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
2. Step-by-step guidance on how to develop OpenHarmony applications with different languages, including ArkTS, Cangjie, Rust, etc.
3. Step-by-step guidance on building an scalable concurrent data structure in OpenHarmony with formal methods.
4. Introduction of the Eclipse Oniro in Europe, which hosts the code and repositories for add-ons and enhancements to the OpenHarmony project.
5. Demonstrating how OpenHarmony enables novel research ideas and supports reliable experimentation for researchers and system designers.


<div class="callout callout--warning">
    <p><strong>Join us (!!!)</strong>In this tutorial to unlock new opportunities and pave the way for secure, interconnected and efficient mobile systems using OpenHarmony. Prior knowledge of operating systems and basic programming concepts would be beneficial.</p>
</div>

## Organizers

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/liuyutao.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Yutao Liu</strong>
    <p>Yutao Liu is the director of Huawei Dresden Research Center. He received his PhD from Shanghai Jiao Tong University in 2017. Research interests include OS and architecture.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/diogo-behrens.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Diogo Behrens</strong>
    <p>Diogo Behrens is the director of Dresden OS Kernel Lab at HW Dresden Research Center. Before joining HW in 2019, Diogo was software engineer with focus on stream data processing. He holds a PhD from TU Dresden, Germany.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/lixinrui.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Xinrui Li</strong>
    <p>Xinrui Li is a 5th year Ph.D. student in IPADS, Shanghai Jiao Tong University. His research focuses on performance optimization in mobile OS. </p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/magnus-morton.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Magnus Morton</strong>
    <p>Magnus Morton is an expert in the Programming Languages lab at the Huawei Edinburgh Research Centre, specializing in the research and application of Effect Handlers technology in the Cangjie Programming language.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/francesco-pham.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Francesco Pham</strong>
    <p>Francesco is an Open Source Software Engineer and the Committer Representative for the Oniro project, leading Eclipse Oniro for OpenHarmony.</p>
  </div>
</div>

<div class="media-left media-left--tutorial">
  <div class="media-left__image">
    <img src="/imgs/jonathan-schwender.jpg" alt="Description of Image">
  </div>
  <div class="media-left__content">
    <strong>Jonathan Schwender</strong>
    <p>Jonathan Schwender is a software engineer at the Huawei Dresden Research Center. He is now a member of the technical steering committee (TSC) for Servo, a web rendering-engine written in Rust.</p>
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
| **11:30am** | Part 5 & Exercise 5: Introduction to Oniro: OpenHarmony graphics stack and device bring-up *(30min)* | Francesco Pham | [slides]() | [code]() |
| **12:00am** | Research Opportunities & Outlook (Conclusion & Remark) *(10min)* | Yutao Liu | | |
| **5:00pm** | Q/A *(10min)* | All | | |

## Topics Introduction

| **Part 1: Introduction to OpenHarmony** <br />Intro |
| **Part 2: OpenHarmony Application Development 101**<br /> This session provides a hands-on introduction to OpenHarmony application development. Through a practical example, we will explore key aspects of OpenHarmony development, including declarative UI design with ArkTs, utilization of system capabilities such as audio, and multi-device collaboration. |
| **Part 3: Concurrency Research based on OpenHarmony**<br />Intro |
| **Part 4: Cangjie for OpenHarmony Native Application Development**<br />Cangjie is a new, general-purpose programming language developed by Huawei, designed to improve performance and developer productivity. It is intended for a wide range of scenarios, from servers to OpenHarmony mobile phones. <br />In this tutorial, we will present an introduction to the Cangjie Programming language, explaining the basics of  its syntax and semantics, before looking at how Cangjie can be used to build rich OpenHarmony applications. <br />The second part of the tutorial will explore Cangjie's Effect Handlers. Effect handlers are and advanced construct for custom concurrency and programmable control flow. We will show how to use this feature, along with some details of the implementation. We will then look at some more complex and practical uses of Effect Handlers in the OpenHarmony ecosystem, demonstrating the power and flexibility of the feature. |
| **Part 5: Oniro Introduction and Development Guide**<br />Oniro, an open-source project hosted by the Eclipse Foundation, extends OpenHarmony with additional functionalities tailored for global markets. This talk will provide an introduction to the Oniro project, focusing on the OpenHarmony graphics stack and the challenges of enabling new devices. <br />We will explore the architecture of OpenHarmony’s rendering pipeline, including the ArkUI framework, Render Service, and display hardware abstraction. The session will highlight the process of bringing up Oniro/OpenHarmony on new devices, such as the Volla X23 phone and QEMU virtual devices. We will discuss how software rasterization and containerization with LXC facilitated rapid prototyping and deployment. <br />The talk will also feature a hands-on tutorial on building and flashing Oniro/OpenHarmony on a Raspberry Pi and showcase a live demo running on QEMU. Attendees will gain insights into the practical steps of device enablement and the challenges involved in running an open-source OS on diverse hardware. |

## Credits

We thank the following people/organizations for their huge supports for the 1st OpenHarmony Research Tutorial (in no particular order).

* OpenHarmony TSC.
* Ming Fu gives suggestions on the content of this tutorial.
* Yubin Xia gives suggestions on the content of this tutorial.
* Dong Du gives suggestions on the content of this tutorial.
* Jiang Rui gives suggestions on the content of this tutorial.
* Guo Liu (刘果)
* and Others
