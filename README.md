# FarPlaneTwo

[![Build Status](https://jenkins.daporkchop.net/job/PorkStudios/job/FarPlaneTwo/job/master/badge/icon)](https://jenkins.daporkchop.net/job/PorkStudios/job/FarPlaneTwo/)
![GitHub Code Size](https://img.shields.io/github/languages/code-size/PorkStudios/FarPlaneTwo)
![Lines of Code](https://img.shields.io/tokei/lines/github/PorkStudios/FarPlaneTwo)
[![Discord](https://img.shields.io/discord/428813657816956929?color=7289DA&label=Join%20our%20Discord)](https://discord.gg/FrBHHCk)
[![Patreon](https://img.shields.io/badge/dynamic/json?color=ff424d&label=Patreon%20Supporters&query=data.attributes.patron_count&suffix=%20patrons&url=https%3A%2F%2Fwww.patreon.com%2Fapi%2Fcampaigns%2F727078)](https://www.patreon.com/DaPorkchop_)

---

## 🌍 What is FarPlaneTwo?

**FarPlaneTwo** is a powerful Minecraft mod that implements a Level-of-Detail (LoD) terrain renderer. It allows for unprecedented render distances and seamless terrain viewing — pushing Minecraft far beyond its default limitations.

The name pays homage to [CWGFarPlaneView](https://www.curseforge.com/minecraft/mc-mods/cwg-far-plane-view), an addon for CubicWorldGen and Cubic Chunks that inspired this project.

> ⚠️ **Warning:** This mod is **work-in-progress** and may be unstable. Use at your own risk.

📖 **Make sure to read the [FAQ](https://github.com/PorkStudios/FarPlaneTwo/wiki/FAQ) before reporting issues.**

---

## 🚀 Installation Guide

> ⚠️ **FarPlaneTwo is for Minecraft 1.12.2 using Forge.** Support for newer versions is planned but not yet available.

### Prerequisites

1. Install [Minecraft Forge 1.12.2](https://files.minecraftforge.net/net/minecraftforge/forge/index_1.12.2.html).
2. Download the **latest build** of FarPlaneTwo from [Jenkins](https://jenkins.daporkchop.net/job/PorkStudios/job/FarPlaneTwo/job/master/).
3. Download the following **dependencies**:
   - [ForgeRocks](https://www.curseforge.com/minecraft/mc-mods/forgerocks)
   - [Mixin Compatibility](https://www.curseforge.com/minecraft/mc-mods/mixin-0-7-0-8-compatibility)

> ✅ **Recommended:** Use with Cubic Chunks + Cubic WorldGen for best visual fidelity.

- [Cubic Chunks (Jenkins)](https://jenkins.daporkchop.net/job/OpenCubicChunks/job/CubicChunks/)
- [Cubic WorldGen (Jenkins)](https://jenkins.daporkchop.net/job/OpenCubicChunks/job/CubicWorldGen/)

📌 *Note:* **Cubic Chunks already includes Mixin. Do not install both.**

### Finding the Right Download

When accessing the Jenkins pages, look for sections titled:

> `Last Successful Artifacts`

Click the topmost `.jar` file listed there, as shown below:

![Example Jenkins Artifact](https://user-images.githubusercontent.com/25571687/119328744-49aa7e00-bc39-11eb-827f-f44611c8ae4e.png)

---

## 🎯 Project Goals

FarPlaneTwo aims to:

- Support render distances of **100,000+ blocks**
- Maintain performance loss under **25%** even on low-end integrated graphics (e.g., Intel i5-2520M)
- Achieve **compatibility with Cubic Chunks**
- Be reasonably **mod-compatible** with existing Forge mods

---

## ⚙️ Technical Insight

This mod explores **unsafe and high-performance techniques**, such as:

- Off-heap memory management for rendering structures (e.g., [`FarRenderTree.java`](https://github.com/PorkStudios/FarPlaneTwo/blob/master/src/main/java/net/daporkchop/fp2/mode/common/client/FarRenderTree.java))
- Custom LoD-based terrain rendering pipeline

> In future versions, more technical documentation and architectural breakdowns will be added.

---

## 💬 Join the Community

- 💬 Chat with us on [Discord](https://discord.gg/FrBHHCk)
- 🧠 Read the [Wiki](https://github.com/PorkStudios/FarPlaneTwo/wiki)
- 💖 Support on [Patreon](https://www.patreon.com/DaPorkchop_)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
© 2020–2021 DaPorkchop_

---