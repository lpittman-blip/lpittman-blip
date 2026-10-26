<a href="https://artemisai-bycutlineindustries.studio"><img src="assets/banner-business.png" width="100%" alt="Cutline Industries: home of Artemis AI. AI training and infrastructure, built and shipped."></a>

<p align="center">
  <a href="https://artemisai-bycutlineindustries.studio"><img alt="Website: artemisai-bycutlineindustries.studio" src="https://img.shields.io/badge/Website-artemisai--bycutlineindustries.studio-3279f9?style=for-the-badge&labelColor=0d0e11"></a>
  <a href="https://artemisai-bycutlineindustries.studio/portfolio/"><img alt="Portfolio: Latoya Pittman" src="https://img.shields.io/badge/Portfolio-Latoya_Pittman-5a3fe0?style=for-the-badge&labelColor=0d0e11"></a>
  <a href="https://github.com/Cutline-industries/artemis-567885"><img alt="Open source: artemis-567885" src="https://img.shields.io/badge/Open_source-artemis--567885-22d3ee?style=for-the-badge&labelColor=0d0e11&logo=github&logoColor=white"></a>
</p>

## Cutline Industries LLC

I'm **Latoya Pittman**, founder of **Cutline Industries LLC**. We build AI systems end to end: the model code, the training runs on rented GPUs, and the cloud infrastructure that keeps them safe and cheap. Our flagship is **[Artemis AI](https://artemisai-bycutlineindustries.studio)**.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🛰️ Artemis AI <sub><code>flagship</code></sub></h3>
      The Artemis AI website, with chat, products and account pages.<br><br>
      <a href="https://artemisai-bycutlineindustries.studio"><img alt="Visit Artemis AI" src="https://img.shields.io/badge/Visit-Artemis_AI-3279f9?style=for-the-badge&labelColor=0d0e11"></a>
    </td>
    <td width="50%" valign="top">
      <h3>🧠 Artemis 567885 <sub><code>open source</code></sub></h3>
      A self-expanding sparse Mixture-of-Experts engine in PyTorch. It grew from 1 to 12 layers over 115 supervised cycles.<br><br>
      <a href="https://github.com/Cutline-industries/artemis-567885"><img alt="View the repo" src="https://img.shields.io/badge/View-repo-22d3ee?style=for-the-badge&labelColor=0d0e11&logo=github&logoColor=white"></a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🖥️ Ops Dashboard and Ops Terminal</h3>
      A secured ops dashboard on Azure Container Apps, plus a sandboxed command API for agents with an audit log.
    </td>
    <td width="50%" valign="top">
      <h3>💸 Cost-capped GPU training</h3>
      Every run gets a hard dollar cap, a kill timer, a self-destruct, and teardown verified by instance ID.
    </td>
  </tr>
</table>

<img src="assets/divider.svg" width="100%" alt="">

### Shipped and measured

- **[Artemis 567885](https://github.com/Cutline-industries/artemis-567885)**: a CPU-first Top-K sparse Mixture-of-Experts transformer in PyTorch with a **self-expanding engine**. It adds experts, layers and capacity when training stalls, and a supervisor rolls back any change that breaks. Over 115 supervised cycles it grew from 1 layer to 12 layers and 93 experts, and eval loss went from 0.0965 to 0.0259. One cycle timed out and rolled back cleanly. Development happens in stacked PRs, and every number has a log.
- **Byte-level language field (no tokenizer)**: raw bytes streamed over HTTP Range plus a Fourier position code, fed through causal MoE blocks. On 1× RTX 4070 it reached **1.662 bits/byte** on held-out text, against 4.619 for a unigram baseline and 2.075 with no position input. Measured spend was $0.03.
- **Training on rented GPUs**: a 48.8M-parameter dense Artemis LM trained on 1× RTX A6000 for 50 minutes (374M tokens). Held-out web text went from 3.293 to 1.191 bits/byte, and the Artemis docs from 4.036 to 1.374. Measured spend was $0.44.
- **Fine-tuning pipeline with cost guards**: QLoRA fine-tunes of a 7B model and a 30B model on 2-GPU rented instances. Every run has a hard dollar cap ($5 and $15), a host-side kill timer, an on-instance self-destruct, and teardown verified by instance ID. Real spend was $0.53 and $1.08.
- **Ops dashboard on Azure**: a password-protected, trading-terminal-style dashboard on Azure Container Apps. It uses bcrypt login, signed sessions, a strict CSP, rate limits and Blob-backed daily snapshots, and refreshes every morning. I also built an **Ops Terminal** for it: a sandboxed command API for agents with a JSON in/out format, per-command timeouts, a command policy, rate limits, secret redaction and an audit log.
- **Forge**: a code-hosting platform I'm building the way large Git hosts are built. It has a Rails monolith; Go services for the API gateway, realtime and Git RPC; quorum-based Git ref replication; Rust trigram code search; and a React UI kit.

<p align="center"><img src="assets/measured.png" width="100%" alt="Measured results: self-expanding MoE engine eval loss 0.0965 to 0.0260; byte-level MoE LM 1.761 bits per byte held-out vs 4.581 unigram; dense LM GPU run 3.293 to 1.191 bits per byte; physics sandbox relative L2 0.0077 vs 0.2497 baseline"></p>

<img src="assets/divider.svg" width="100%" alt="">

<img src="assets/divider.svg" width="100%" alt="">

### Stack

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3279f9?style=flat-square&labelColor=0d0e11"> <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-3279f9?style=flat-square&labelColor=0d0e11"> <img alt="CUDA" src="https://img.shields.io/badge/CUDA-3279f9?style=flat-square&labelColor=0d0e11"> <img alt="QLoRA / PEFT" src="https://img.shields.io/badge/QLoRA_/_PEFT-3279f9?style=flat-square&labelColor=0d0e11"> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-5a3fe0?style=flat-square&labelColor=0d0e11"> <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-5a3fe0?style=flat-square&labelColor=0d0e11"> <img alt="React" src="https://img.shields.io/badge/React-5a3fe0?style=flat-square&labelColor=0d0e11"> <img alt="Go" src="https://img.shields.io/badge/Go-22d3ee?style=flat-square&labelColor=0d0e11"> <img alt="Rust" src="https://img.shields.io/badge/Rust-22d3ee?style=flat-square&labelColor=0d0e11"> <img alt="Ruby on Rails" src="https://img.shields.io/badge/Ruby_on_Rails-22d3ee?style=flat-square&labelColor=0d0e11"> <img alt="Azure Container Apps" src="https://img.shields.io/badge/Azure_Container_Apps-6aa0ff?style=flat-square&labelColor=0d0e11"> <img alt="Azure Blob" src="https://img.shields.io/badge/Azure_Blob-6aa0ff?style=flat-square&labelColor=0d0e11"> <img alt="Docker" src="https://img.shields.io/badge/Docker-6aa0ff?style=flat-square&labelColor=0d0e11"> <img alt="Linux" src="https://img.shields.io/badge/Linux-6aa0ff?style=flat-square&labelColor=0d0e11"> <img alt="Bash" src="https://img.shields.io/badge/Bash-6aa0ff?style=flat-square&labelColor=0d0e11">
</p>

### How I work

Measure first, label estimates, and keep negative results. Every GPU run gets a price cap, a time limit and a verified teardown. Defaults stay off until a test proves the old path still holds.

### What I'm looking for

Roles on **AI training and infrastructure teams**: model and training-systems work, GPU and cluster efficiency, and the tooling that keeps large runs safe and cheap.

<img src="assets/divider.svg" width="100%" alt="">

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=lpittman-blip&show_icons=true&hide_border=true&bg_color=0d0e11&title_color=6aa0ff&text_color=b4b9c4&icon_color=22d3ee&disable_animations=true" alt="GitHub stats for lpittman-blip">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=lpittman-blip&layout=compact&hide_border=true&bg_color=0d0e11&title_color=6aa0ff&text_color=b4b9c4&disable_animations=true" alt="Top languages for lpittman-blip">
</p>

<p align="center">
  <a href="https://artemisai-bycutlineindustries.studio"><b>Cutline Industries LLC</b> · artemisai-bycutlineindustries.studio</a>
</p>
