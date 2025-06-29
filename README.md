# Vehicle-Wise: 高性能、高扩展性的车联网SaaS平台解决方案

[![Go Version](https://img.shields.io/badge/Go-1.18%2B-blue.svg)](https://golang.org/)
[![Flutter Version](https://img.shields.io/badge/Flutter-3.x-blue.svg)](https://flutter.dev/)
[![Vue Version](https://img.shields.io/badge/Vue-3.x-brightgreen.svg)](https://vuejs.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**[English](README.en.md) | 简体中文**

---

## 声明

**本项目并非一个开源项目，而是我独立设计并领导开发的一套成熟、稳定、经过商业验证的北斗/GPS车联网SaaS平台的解决方案展示。**

我创建这个仓库的目的，是希望通过最直接的方式，向潜在的商业伙伴展示我们的技术实力和产品价值，寻求**OEM合作、私有化部署、技术咨询**等多种形式的商业合作。

如果您是**北斗/GPS硬件厂商、行业解决方案提供商、大型车队管理者**，或是任何对构建高效车联网平台有需求的朋友，相信我们的技术与产品能为您带来巨大的价值。

> **寻求合作？请直接联系我：**
>
> *   **邮箱：** `qiueye@gmail.com`
> *   **邮箱：** `78282385@qq.com`
> *   **微信：** `waynerQiu` (请注明“GitHub车联网合作”)

---

## 平台概述 (Platform Overview)

**Vehicle-Wise** 是一套专为现代物流、车辆租赁、集团车队、道路救援等场景设计的综合性车辆监管与服务平台。我们致力于通过软硬件的深度结合，提供从数据采集、实时监控、大数据分析到业务流程优化的全链路解决方案，帮助企业实现**降本增效、安全合规、精细化运营**。

**核心亮点：**

*   **企业级稳定可靠：** 平台已在**数十家企业客户**的生产环境中稳定运行超过半年，管理着**近千台**在线设备，其稳定性与可靠性得到了充分检验。
*   **全终端覆盖：** 提供 **Web管理端、小程序、Flutter App (iOS & Android)**，满足管理人员、车队司机等不同角色的使用需求。
*   **开放与集成：** 提供标准的 **GPS数据API**，方便与您现有的ERP、TMS、OA等系统无缝集成，打破信息孤岛。
*   **灵活部署：** 同时支持 **SaaS订阅** 和 **私有化部署**，满足不同规模和安全等级的企业需求。
*   **国际化支持：** 同时支持 **中文**、**英文**、**菲律宾语**、**泰语**、**马来语**、**印度语**等多国家语言支持。

---

## 技术架构与亮点 (Technical Architecture & Highlights)

我们采用业界领先的云原生技术栈，构建了一套高可用、高扩展性的微服务架构。

### **后端核心 (Backend Core)**

*   **高性能协议网关:**
    *   **技术:** 采用 **Go语言** 构建，充分利用其原生并发优势，为海量设备连接提供坚实基础。
    *   **性能:** 经压力测试，单机可稳定支撑 **15~50万+** 设备TCP/UDP长连接并发，数据转发延迟低于10ms。
*   **强大的协议兼容性:**
    *   **标准协议:** 深度支持 **JT/T 808-2019**, **GT06**, **谷米(GT02D)** 等行业标准协议。
    *   **魔改与私有协议:** 具备丰富的协议逆向与适配经验，能快速兼容市面上各种**“魔改版JT808”**及厂商私有协议。 **(这是我们解决实际问题能力的重要体现)**
*   **稳健的中间件:**
    *   **数据存储:** **MySQL** (业务数据) + **InfluxDB** (海量轨迹时序数据) + **Redis** (高速缓存与消息队列)，实现了最优的数据读写与存储成本平衡。
*   **实时双向通信:**
    *   采用 **Socket.IO** 实现前端与后端的数据实时推送，确保地图上车辆移动的平滑性、报警信息的即时性。

### **前端应用 (Frontend Applications)**

*   **PC Web管理端:**
    *   **技术:** 采用 **Vue 3 + Vite + TypeScript + Element Plus** 构建，提供强大的数据管理与可视化能力。
*   **移动端 (App & 小程序):**
    *   **App:** 使用 **Flutter** 开发，一套代码覆盖 **iOS** 和 **Android** 两大平台，保证体验一致性与开发效率。
    *   **小程序:** 使用 **Vue** (uni-app或原生) 开发，轻量、便捷，便于快速分享与传播。
*   **强大的地图引擎支持:**
    *   **多地图切换:** 平台内置地图抽象层，支持一键切换**高德地图、百度地图、Google Maps、OpenStreetMap、Mapbox**等多种地图服务，满足国内及海外业务需求。

---

## 完备的核心功能 (Comprehensive Core Features)

我们的平台已覆盖车联网行业所有主流核心功能，并针对细节进行了深度优化：

*   **实时监控：** 车辆列表、精准实时定位、多车同屏监控、实时时速展示。
*   **历史轨迹：** 轨迹数据长期存储、高效率查询、平滑轨迹回放、支持拖拽进度与多倍速播放。
*   **电子围栏：** 支持多边形、圆形、线路等多种围栏类型，实现进出、偏航、超速等多维度报警。
*   **指令与控制：** 支持远程断油电、设备重启、参数设置、拍照、监听等下发指令（需硬件支持）。
*   **报警中心：** 统一管理所有报警信息（如SOS、超速、离线、围栏、碰撞、震动等），支持多渠道推送。
*   **数据报表：** 提供里程、油耗、停留、报警等多维度的数据统计与分析报表，支持导出。
*   **权限管理：** 精细化的多级用户与角色权限管理体系，满足集团型企业组织架构需求。

**我们相信，真实的平台交互体验远胜于静态的截图。为了保护我们的知识产权并为您提供最直观的感受，我们诚邀您联系我们进行一次在线实时演示(Live Demo)。在演示中，我们可以深入探讨您的具体业务场景和需求。**

---

## 商业合作模式 (Business Cooperation Models)

我们深知不同伙伴有不同的需求，因此提供灵活多样的合作模式：

1.  **OEM / 定制合作 (For Hardware Manufacturers & Solution Providers)**
    *   **内容：** 我们提供成熟的SaaS平台作为您的“软件大脑”，可定制品牌Logo、UI风格，甚至深度定制功能。
    *   **优势：** 让您专注于硬件或行业渠道，我们解决所有技术难题，助您快速推出自有品牌的软件产品。

2.  **私有化部署 (For Large Enterprises & Government)**
    *   **内容：** 我们提供平台的全套源码和专业的部署服务，将系统部署在您指定的服务器或内网环境中。
    *   **优势：** 数据100%私有可控，满足最高安全合规要求，支持无限制的二次开发。

3.  **GPS数据API服务**
    *   **内容：** 如果您已有自己的业务系统，只需车辆定位数据，我们可提供稳定、高速的API接口服务。
    *   **优势：** 按需付费，成本低廉，快速为您的现有系统插上“眼睛”。

4.  **技术咨询与顾问服务**
    *   **内容：** 凭借我们丰富的架构和实战经验，为您提供协议适配、性能优化、技术选型等顾问服务。

---

## 关于我 & 联系方式 (About Me & Contact)

我是一名热爱技术的连续创业者和全栈架构师，在互联网及物联网领域深耕多年。我坚信优秀的技术终将创造巨大的商业价值。

如果您对我的项目和经验感兴趣，或是有任何合作的可能性，非常欢迎与我取得联系。让我们一起，用技术驱动行业变革。

> *   **邮箱：** `qiueye@gmail.com`
> *   **邮箱：** `78282385@qq.com`
> *   **微信：** `waynerQiu` (请注明“GitHub车联网合作”)
