# Vehicle-Wise: A High-Performance, Scalable Telematics SaaS Platform Solution

[![Go Version](https://img.shields.io/badge/Go-1.18%2B-blue.svg)](https://golang.org/)
[![Flutter Version](https://img.shields.io/badge/Flutter-3.x-blue.svg)](https://flutter.dev/)
[![Vue Version](https://img.shields.io/badge/Vue-3.x-brightgreen.svg)](https://vuejs.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**English | [简体中文](README.md)**

---

## Disclaimer

**This is NOT an open-source project. It is a solution showcase for a mature, stable, and commercially-proven Telematics SaaS platform that I have independently designed and developed.**

The purpose of this repository is to demonstrate our technical capabilities and product value to potential business partners in the most direct way possible. We are actively seeking various forms of business collaboration, such as **OEM partnerships, private deployments, and technical consulting**.

If you are a **GPS hardware manufacturer, an industry solution provider, a large-scale fleet manager**, or anyone in need of a powerful telematics platform, we are confident that our technology and products can bring significant value to your business.

> **Seeking Collaboration? Contact me directly:**
>
> *   **Email:** `qiueye@gmail.com`
> *   **Email:** `78282385@qq.com`
> *   **WeChat:** `waynerQiu` (Please specify "GitHub Telematics Collab")

---

## Platform Overview

**Vehicle-Wise** is a comprehensive vehicle telematics and service platform designed for modern logistics, vehicle leasing, corporate fleets, and roadside assistance scenarios. Through the deep integration of software and hardware, we provide an end-to-end solution—from data acquisition and real-time monitoring to big data analytics and business process optimization—to help enterprises achieve **cost reduction, efficiency improvement, security compliance, and fine-grained operations**.

**Core Highlights:**

*   **Enterprise-Grade Stability:** The platform has been running stably in the production environments of **dozens of corporate clients** for over six months, managing **nearly a thousand** online devices. Its reliability has been thoroughly tested and proven.
*   **Full-Terminal Coverage:** We provide a **Web-based admin panel, Mini-Program, and a Flutter App (iOS & Android)** to meet the needs of various roles, including managers and drivers.
*   **Open & Integrated:** A standard **GPS Data API** is available to seamlessly integrate with your existing ERP, TMS, OA, or other systems, breaking down information silos.
*   **Flexible Deployment:** We support both **SaaS subscriptions** and **private deployments** to accommodate businesses of different scales and security requirements.
*   **Internationalization support: ** Simultaneous support for many languages ​​such as **Chinese**, **English**, **Filipino**, **Thai**, **Malay**, **Hindi** and other countries.

---

## Technical Architecture & Highlights

We leverage a cutting-edge, cloud-native tech stack to build a highly available and scalable microservices architecture.

### **Backend Core**

*   **High-Performance Protocol Gateway:**
    *   **Technology:** Built with **Go**, fully leveraging its native concurrency advantages to provide a solid foundation for massive device connections.
    *   **Performance:** Stress tests show a single server can stably handle **150,000 to 500,000+** concurrent TCP/UDP long-lived connections with data forwarding latency under 10ms.
*   **Robust Protocol Compatibility:**
    *   **Standard Protocols:** In-depth support for industry standards like **JT/T 808-2019**, **GT06**, and **Gosafe (GT02D)**.
    *   **Custom & Private Protocols:** We have extensive experience in reverse-engineering and adapting protocols, enabling us to quickly support various **customized versions of JT808** and other proprietary manufacturer protocols. **(This is a testament to our practical problem-solving capabilities.)**
*   **Solid Middleware Stack:**
    *   **Data Storage:** A combination of **MySQL** (for business data), **InfluxDB** (for massive time-series trajectory data), and **Redis** (for high-speed caching and message queuing) achieves an optimal balance of read/write performance and storage cost.
*   **Real-time Bidirectional Communication:**
    *   Utilizes **Socket.IO** for real-time data push between the frontend and backend, ensuring smooth vehicle movement on maps and instant alert notifications.

### **Frontend Applications**

*   **PC Web Admin Panel:**
    *   **Technology:** Built with **Vue 3 + Vite + TypeScript + Element Plus** to provide powerful data management and visualization capabilities.
*   **Mobile (App & Mini-Program):**
    *   **App:** Developed with **Flutter**, covering both **iOS** and **Android** with a single codebase for a consistent user experience and high development efficiency.
    *   **Mini-Program:** Developed with **Vue** (uni-app or native) for a lightweight and convenient user experience, easy to share and distribute.
*   **Powerful Map Engine Support:**
    *   **Multi-Map Switching:** A built-in map abstraction layer allows for one-click switching between various map services, including **GaoDe Maps, Baidu Maps, Google Maps, OpenStreetMap, and Mapbox**, to meet both domestic and international business needs.

---

## Comprehensive Core Features

Our platform covers all mainstream core functions in the telematics industry, with deep optimization in every detail:

*   **Real-time Monitoring:** Vehicle list, precise real-time positioning, multi-vehicle monitoring on a single screen, and real-time speed display.
*   **Historical Trajectory:** Long-term storage of trajectory data, high-efficiency querying, smooth track playback with support for progress dragging and multiple playback speeds.
*   **Geo-fencing:** Supports various fence types including polygons, circles, and routes, enabling multi-dimensional alerts for entry/exit, route deviation, and over-speeding.
*   **Commands & Control:** Supports remote commands such as fuel/power cut-off, device reboot, parameter setting, photo capture, and audio monitoring (hardware-dependent).
*   **Alert Center:** Centralized management of all alert information (e.g., SOS, speeding, offline, geo-fence, collision, vibration) with multi-channel push notifications.
*   **Data Reports:** Provides multi-dimensional data statistics and analysis reports for mileage, fuel consumption, stops, and alerts, with export functionality.
*   **Permission Management:** A fine-grained, multi-level user and role permission management system to meet the needs of large corporate organizational structures.

**We believe a live, interactive platform experience is far more compelling than static screenshots. To protect our intellectual property and offer you the most direct insight, we cordially invite you to contact us for a live online demo. During the demo, we can have an in-depth discussion about your specific business scenarios and requirements.**

---

## Business Cooperation Models

We understand that different partners have different needs, which is why we offer a variety of flexible cooperation models:

1.  **OEM / Customization (For Hardware Manufacturers & Solution Providers)**
    *   **What we offer:** A mature SaaS platform to act as your "software brain," customizable with your brand logo, UI style, and even deep feature customization.
    *   **Your advantage:** Focus on your hardware or industry channels while we handle all the technical challenges, helping you launch your own branded software product quickly.

2.  **Private Deployment (For Large Enterprises & Government)**
    *   **What we offer:** The complete source code of the platform and professional deployment services to install the system on your designated servers or private network.
    *   **Your advantage:** 100% private and controllable data, meeting the highest security and compliance standards, with support for unlimited secondary development.

3.  **GPS Data API Service**
    *   **What we offer:** If you already have your own business system and just need vehicle location data, we can provide a stable, high-speed API service.
    *   **Your advantage:** Pay-as-you-go, cost-effective, and a quick way to empower your existing systems with real-time visibility.

4.  **Technical Consulting & Advisory**
    *   **What we offer:** Leveraging our extensive architectural and practical experience, we provide consulting services such as protocol adaptation, performance optimization, and technology selection for your existing technical teams.

---

## About Me & Contact

I am a passionate technology enthusiast, serial entrepreneur, and full-stack architect with many years of deep experience in the Internet and IoT fields. I firmly believe that excellent technology ultimately creates immense business value.

If you are interested in my project and experience, or if there is any possibility for collaboration, I warmly welcome you to get in touch. Let's drive industry transformation with technology, together.

> *   **Email:** `qiueye@gmail.com`
> *   **Email:** `78282385@qq.com`
> *   **WeChat:** `waynerQiu` (Please specify "GitHub Telematics Collab")
