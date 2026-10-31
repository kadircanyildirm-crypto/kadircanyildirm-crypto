<div align="center">

<img src="assets/hero.svg?v=4" alt="Kadir Can Yıldırım — Backend &amp; Systems Engineer · AI Specialist" width="100%"/>

<a href="https://github.com/search?q=author%3Akadircanyildirm-crypto+is%3Apr+is%3Amerged+org%3Anasa+org%3Acvmfs&type=pullrequests"><img src="assets/upstream-band.svg?v=4" alt="Merged upstream — NASA F´ and spacewasm, CERN CernVM-FS" width="100%"/></a>

<img src="assets/status.svg?v=4" alt="Currently building wardyn" width="100%"/>

</div>

<br/>

I build systems software in Rust — infrastructure that sits close to the kernel and the network, where security and privacy are design constraints rather than features bolted on afterwards.

Backend and systems engineer, studying Software Development at Anadolu University. My work sits where distributed systems, system-level security and AI infrastructure meet: middleware that has to stay up, peer-to-peer networks that have to stay reachable, and kernel-level enforcement that has to stay honest. I take on the backend bottlenecks other people route around.

<br/>

<div align="center">
<a href="https://doi.org/10.22541/essoar.15008581/v1"><img src="assets/paper.svg?v=4" alt="Research preprint — An Independent Evaluation of Surya's Solar Flare Forecasting: Cheap Baselines Match a 366M-Parameter Foundation Model (ESS Open Archive, 2026)" width="100%"/></a>
</div>

An independent evaluation of Surya, the 366M-parameter heliophysics foundation model released by NASA and IBM. I ran the released checkpoint with the authors' own inference code on 1,146 forecast hours streamed from roughly 700 GB of raw SDO data, and scored the cheap baselines the benchmark never reports: an 11-feature logistic regression over past GOES X-ray flux matches the model, and the benchmark's effective sample turns out too small to rank either. Every number in the manuscript is recomputed by `verify_paper.py` — 161 of 161 claims.

**[Preprint](https://doi.org/10.22541/essoar.15008581/v1)** · ESS Open Archive · **[heliofloor](https://github.com/kadircanyildirm-crypto/heliofloor)** · code and data · **[Zenodo](https://doi.org/10.5281/zenodo.22905499)** · [ORCID](https://orcid.org/0009-0008-5098-2547)

<br/>

<div align="center">
<img src="assets/pipeline-wardyn.svg?v=4" alt="wardyn architecture — runtime containment for AI coding agents" width="100%"/>
</div>

A kernel-level warden for AI coding agents. eBPF LSM hooks and tracepoints watch every file, exec and socket the agent touches, and refuse the ones policy forbids before the syscall completes — no kernel module, no agent cooperation required.

**[wardyn](https://github.com/kadircanyildirm-crypto/wardyn)** · `Rust` · `AGPL-3.0` · open source

<br/>

<div align="center">
<img src="assets/code.svg?v=4" alt="Source excerpt from wardyn-ebpf — the LSM file_open enforcement path" width="100%"/>
</div>

<br/>

### Focus

**Runtime containment** — kernel-level wardens and sealed execution environments for autonomous AI agents, enforced below the process rather than negotiated with it.

**Verifiable privacy** — transparent L7 data-masking proxies and zero-knowledge proofs, so a result can be trusted without trusting the machine that produced it.

**Decentralised transport** — offline disaster-communication nodes and enterprise API gateways coordinated by gossip protocols and CRDTs, built to survive the network being wrong.

<br/>

<div align="center">
<img src="assets/stack.svg?v=4" alt="Component schedule — Rust, Python, Go, Kotlin, eBPF, Kubernetes, CRDT, Ed25519, zkVM, PostgreSQL" width="100%"/>
</div>

Rust for the parts that must not fail, Python and Go for the parts that must move quickly. Everything ships containerised and orchestrated — Docker and Kubernetes, minimal egress, fault tolerance assumed rather than added later. Working is the floor; deterministic and stable at the edge of the machine's capacity is the bar.

<br/>

<div align="center">
<img src="assets/register.svg?v=4" alt="Project register — seven open-source systems: wardyn, low-latency-matching-engine, quaestor, petek, heliofloor, nabd, spacewasm-crossbuild" width="100%"/>
</div>

From a kernel warden to an exchange matching engine, the through-line is the same: push the boundary where network optimisation meets machine learning, and keep latency and trust on the right side of it. Every one of these is public — read the code.

**[wardyn](https://github.com/kadircanyildirm-crypto/wardyn)** · **[low-latency-matching-engine](https://github.com/kadircanyildirm-crypto/low-latency-matching-engine)** · **[quaestor](https://github.com/kadircanyildirm-crypto/quaestor)** · **[petek](https://github.com/kadircanyildirm-crypto/petek)** · **[heliofloor](https://github.com/kadircanyildirm-crypto/heliofloor)** · **[nabd](https://github.com/kadircanyildirm-crypto/nabd)** · **[spacewasm-crossbuild](https://github.com/kadircanyildirm-crypto/spacewasm-crossbuild)**

<br/>

<div align="center">
<img src="assets/upstream.svg?v=4" alt="Upstream record — thirteen patches merged into NASA F´, NASA spacewasm and CERN CernVM-FS" width="100%"/>
</div>

Thirteen patches merged into code other people's missions depend on: build-system and deployment correctness in **F´**, the NASA flight software framework flown on the Ingenuity Mars helicopter; decoder, host-interface and build fixes in **spacewasm**, NASA's flight-compliant WebAssembly interpreter; and toolchain, logging and test-suite fixes in **CernVM-FS**, the filesystem CERN uses to distribute LHC experiment software to computing sites worldwide. Reading an unfamiliar build system until the failure is obvious is the same work as reading a kernel path — only with a stricter review queue. More are in review.

**[nasa/fprime](https://github.com/nasa/fprime)** · [#5675](https://github.com/nasa/fprime/pull/5675) · [#5590](https://github.com/nasa/fprime/pull/5590) · [#5576](https://github.com/nasa/fprime/pull/5576) · [#5571](https://github.com/nasa/fprime/pull/5571) · [#5559](https://github.com/nasa/fprime/pull/5559)<br/>
**[nasa/spacewasm](https://github.com/nasa/spacewasm)** · [#190](https://github.com/nasa/spacewasm/pull/190) · [#154](https://github.com/nasa/spacewasm/pull/154) · [#153](https://github.com/nasa/spacewasm/pull/153) · [#152](https://github.com/nasa/spacewasm/pull/152)<br/>
**[cvmfs/cvmfs](https://github.com/cvmfs/cvmfs)** · [#4407](https://github.com/cvmfs/cvmfs/pull/4407) · [#4396](https://github.com/cvmfs/cvmfs/pull/4396) · [#4392](https://github.com/cvmfs/cvmfs/pull/4392) · **[cvmfs/doc-cvmfs](https://github.com/cvmfs/doc-cvmfs)** · [#265](https://github.com/cvmfs/doc-cvmfs/pull/265)

<br/>

I'm open to systems and infrastructure work — Rust services, kernel and network-level tooling, distributed architecture, and security engineering. If you need help or know someone who does, I'd appreciate an introduction.

`kadir.can.yildirm@gmail.com`

<br/>

<div align="center">

<img src="assets/footer.svg?v=4" alt="Sheets 01 to 06 · revision 2026.10 · Anadolu University" width="100%"/>

</div>
