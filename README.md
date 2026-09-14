<h1 align="center">Otoniel Pérez</h1>

<p align="center">
  <b>Backend Software Engineer (.NET)</b><br>
  Gran Canaria, Spain
</p>

<p align="center">
  <a href="https://otonielpv.github.io"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-otonielpv.github.io-0F766E?style=for-the-badge"></a>
  <a href="https://linkedin.com/in/otoniel-p%C3%A9rez-577558188"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:otonielcuentas@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

---

I build the parts of a system that other teams build on top of. Shared libraries, internal APIs, deployment tooling and the observability that tells you when any of it breaks. Day to day that means **.NET and Azure** on a cross-cutting platform team — designing core services, keeping a large codebase modern (.NET Core 3.1 → .NET 10), and wiring up distributed, event-driven flows.

Outside work I build **realtime audio and video software**. That started with timing systems for rally motorsport in 2016 and turned into [LibreTracks](https://github.com/otonielpv/LibreTracks), a multitrack DAW with a C++ audio engine that now runs on five platforms. Different domain, same problem. A lot of moving parts have to stay correct under a deadline that does not wait for you, a HTTP timeout in one case and a 5 ms audio callback in the other.

<br>

## 🎛️ LibreTracks

> A multitrack DAW and live-playback workstation for Windows, macOS, Linux, Android and iOS.<br>
> Free and open source · **[libretracks.com](https://libretracks.com)**

<p align="center">
  <a href="https://github.com/otonielpv/LibreTracks">
    <img src="https://raw.githubusercontent.com/otonielpv/otonielpv/main/assets/libretracks-timeline.png" alt="LibreTracks arrangement view" width="100%">
  </a>
</p>

<p align="center">
  <img alt="Stars" src="https://img.shields.io/github/stars/otonielpv/LibreTracks?style=flat-square&color=EAB308">
  <img alt="Release" src="https://img.shields.io/github/v/release/otonielpv/LibreTracks?style=flat-square&color=0F766E">
  <img alt="Downloads" src="https://img.shields.io/github/downloads/otonielpv/LibreTracks/total?style=flat-square&color=0F766E">
  <img alt="Commits" src="https://img.shields.io/github/commit-activity/t/otonielpv/LibreTracks?style=flat-square&color=64748B">
</p>

LibreTracks is built for musicians playing live to backing tracks. Non-destructive arrangement, section jumps and vamps that land on the beat, per-region transpose and time-stretch, a click and guide-voice bus, and a browser remote so the player can drive the session from a tablet on stage.

The interesting part is the boundary. Realtime playback lives in a **C++ engine** that must never block or allocate on the audio thread. **Rust** owns the domain model, persistence and orchestration. **React + Tauri** owns editing and presentation. Each layer only knows what it needs to, which is what makes it possible to add features to the UI without putting a click in someone's in-ear monitor.

<table>
<tr>
<td width="50%"><img src="https://raw.githubusercontent.com/otonielpv/otonielpv/main/assets/libretracks-session.png" alt="Session view with clip launcher and mixer"><br><sub><b>Session view</b> — clip launching and mixer</sub></td>
<td width="50%"><img src="https://raw.githubusercontent.com/otonielpv/otonielpv/main/assets/libretracks-remote.png" alt="Browser remote running on a tablet"><br><sub><b>Remote</b> — customisable stage control from any browser</sub></td>
</tr>
</table>

`C++17` · `Rust` · `React 19` · `TypeScript` · `Tauri v2` · `Zustand` · `CMake` · `Android NDK` · `CoreAudio / WASAPI / ASIO / AAudio`

<br>

## Other things I've built

| Project | What it is | Stack |
| --- | --- | --- |
| **[SonyLiveMonitor](https://github.com/otonielpv/SonyLiveMonitor)** | Wireless monitor for Sony mirrorless cameras whose live view keeps running *while the camera records* — plus SD-card browsing and RAW/ARW pull to the phone. Ships a one-click camera patcher for Windows, macOS and Linux. | Kotlin · Android · Sony Camera Remote API |
| **[AI-Tracking-PTZ](https://github.com/otonielpv/AI-Tracking-PTZ)** | Auto-tracking for PTZ cameras: RTSP/NDI capture, YOLO person detection, persistent target selection, ONVIF pan-tilt-zoom driven by a PID loop, MIDI cues out to presentation software. | Python · YOLO · ONVIF · NDI · TensorRT |
| **[REAPER-Live-Remote](https://github.com/otonielpv/REAPER-Live-Remote)** | Touch remote for REAPER so a musician can run backing tracks from a tablet instead of walking back to the laptop mid-set. | JavaScript · REAPER Web API |
| **[Android-NDI-Player](https://github.com/otonielpv/Android-NDI-Player)** | Native NDI receiver for Android — source discovery and fullscreen realtime video over a JNI bridge to the NDI SDK. | C++ · Kotlin · JNI · NDI SDK |
| **[delayed-fade-obs](https://github.com/otonielpv/delayed-fade-obs)** | OBS Studio transition plugin that holds the outgoing scene for a configurable delay before starting the fade. | C · CMake · OBS plugin API |

<br>

## Tech

**Languages**<br>
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)

**Frameworks & runtime**<br>
![.NET](https://img.shields.io/badge/.NET_3.1_→_10-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

**Cloud, DevOps & containers**<br>
![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azuredevops&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Architecture & practices**<br>
`Microservices` · `REST APIs` · `Distributed systems` · `Event-driven architecture` · `CQRS` · `AuthN / AuthZ` · `Centralized configuration` · `TDD` · `Code review` · `Mentoring`

**Observability & applied AI**<br>
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![App Insights](https://img.shields.io/badge/Application_Insights-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
`Azure AI Search` · `RAG` · `LLM integration`

<br>

## Experience

**Backend Engineer / .NET Specialist** — AIDA, Cross-Cutting Team · *July 2022 – Present*<br>
Shared libraries, internal APIs and foundational services used across multiple product teams. Built **DeploymentTool**, an internal platform that standardises and automates deployments across Windows Server and IIS. Designed a **Centralized Configuration API** and took ownership of the corporate **API-key authentication service**. Built a **Streaming API** for realtime event processing and a centralized email delivery service. Set up OpenTelemetry / Application Insights instrumentation, Grafana dashboards and company-wide alerting into Microsoft Teams. Shipped an internal **RAG chatbot** over confidential corporate documentation using Azure AI Search. Mentored software engineering interns.

**Rally Timing Systems — Development & Operations** — A Todo Motor · *2016 – Present*<br>
Timing system used live at motorsport events. Contributed to migrating it from a desktop application to a **Node.js** web platform, applying **TDD** and **CQRS**, and still maintain and operate it during live rallies.

**B.Eng. Computer Engineering** — Universidad de Las Palmas de Gran Canaria (ULPGC) · *2023*

<br>

## Get in touch

**[otonielcuentas@gmail.com](mailto:otonielcuentas@gmail.com)** · **[LinkedIn](https://linkedin.com/in/otoniel-p%C3%A9rez-577558188)** · **[otonielpv.github.io](https://otonielpv.github.io)**

<sub>Spanish (native) · English (upper-intermediate) — Gran Canaria, Spain · open to remote</sub>
