<div align="center">

# Paul Chrétien

**Élève Ingénieur — Télécom Saint-Étienne**  
Systèmes performants · Inférence embarquée · Architecture logicielle

[![LinkedIn](https://img.shields.io/badge/LinkedIn-paul--chretien-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/paul-chretien)
[![Email](https://img.shields.io/badge/Email-paul.chretien.69@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:paul.chretien.69@gmail.com)
[![Location](https://img.shields.io/badge/Lyon%2C_France-📍-lightgrey?style=flat-square)](#)
[![Open to](https://img.shields.io/badge/Open_to-Stage_5_mois_été_2026-22c55e?style=flat-square)](#)

</div>

---

## Projects

### [Word-Waker](https://github.com/paul3ien/Word-waker) — Real-time wake-word daemon for macOS
> *Real-time audio inference pipeline running entirely on Apple Silicon — no server, no latency.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust)
![CoreML](https://img.shields.io/badge/CoreML-0071E3?style=flat-square&logo=apple)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python)
![C++](https://img.shields.io/badge/Objective--C++-00599C?style=flat-square&logo=c%2B%2B)

Lock-free DSP pipeline in Rust feeding a CoreML CNN accelerated on the Apple Neural Engine. Includes a full custom training pipeline (MobileNet-style, 62k params) with cross-validation between Python and Rust inference.

```
Mic → pre-emphasis → FFT (vDSP) → Mel filterbank → MFCC → CoreML (ANE) → sliding vote → UDS
```

| Metric | Value |
|---|---|
| CPU usage | < 0.5% |
| End-to-end latency | < 20 ms |
| ANE inference (P50) | ~17 µs |
| Model AUC-ROC | 0.9993 |
| False Accept Rate | 0.57% |

---

### [LinkUp](https://github.com/paul3ien/LinkUp) — Real-time chat, microservices architecture
> *Full-stack distributed system — from gRPC contracts to Angular UI.*

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=google)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes)

Three decoupled ASP.NET Core 8 services communicating over gRPC, with JWT auth, EF Core migrations, and a full CI/CD pipeline. 69 tests passing across backend (xUnit) and frontend (Jasmine).

```
Angular (gRPC-Web) → AuthService (JWT) ─┐
                                         ├─ gRPC ─→ NotificationService
                   → BusinessService ───┘
```

---

### Log Anomaly Detection — VGAE *(ReachFive POC)*
> *Graph-based behavioral modeling for authentication log analysis.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch)
![PyG](https://img.shields.io/badge/PyG-3C2179?style=flat-square&logo=pyg)

Variational Graph Autoencoder trained on heterogeneous user event graphs (userId, IP, device as nodes). Detects structural outliers via HDBSCAN and behavioral anomalies via reconstruction error. Built with privacy constraints — anonymization and hashing applied before any cloud processing.

---

### [VM Manager](https://github.com/paul3ien/vm-rust-m4) — Ubuntu headless VM on Apple Silicon
> *Thin Rust wrapper around Apple's Virtualization framework — no GUI, serial console only.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust)
![macOS](https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple)

Direct Objective-C FFI bindings to `VZVirtualMachine`, EFI boot with persistent NVRAM, VirtIO serial console with full raw terminal passthrough. ~420 lines of Rust.

---

## Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=paul3ien&show_icons=true&theme=github_dark&hide_border=true&rank_icon=github)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=paul3ien&layout=compact&theme=github_dark&hide_border=true&langs_count=8)

</div>

---

## Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![CoreML](https://img.shields.io/badge/CoreML-0071E3?style=flat-square&logo=apple&logoColor=white)
![ASP.NET](https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=google&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

<div align="center">
<sub>Télécom Saint-Étienne · exchange @ Toyohashi University of Technology 🇯🇵 · open to relocation</sub>
</div>
