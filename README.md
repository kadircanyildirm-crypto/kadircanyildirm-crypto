<div align="center">

<img src="assets/hero.svg" alt="Kadir Can Yıldırım — Systems Engineer, Rust, kernel-level and distributed infrastructure" width="100%"/>

<img src="assets/status.svg" alt="Currently building wardyn" width="100%"/>

</div>

<br/>

I build systems software in Rust — infrastructure that sits close to the kernel and the network, where security and privacy are design constraints rather than features bolted on afterwards.

Backend and systems engineer, studying Software Development at Anadolu University. My work sits where distributed systems, system-level security and AI infrastructure meet: middleware that has to stay up, peer-to-peer networks that have to stay reachable, and kernel-level enforcement that has to stay honest. I take on the backend bottlenecks other people route around.

<br/>

<div align="center">
<img src="assets/pipeline-wardyn.svg" alt="wardyn architecture — runtime containment for AI coding agents" width="100%"/>
</div>

A kernel-level warden for AI coding agents. eBPF LSM hooks and tracepoints watch every file, exec and socket the agent touches, and refuse the ones policy forbids before the syscall completes — no kernel module, no agent cooperation required.

**[wardyn](https://github.com/kadircanyildirm-crypto/wardyn)** · `Rust` · `AGPL-3.0` · open source

<br/>

<div align="center">
<img src="assets/code.svg" alt="Source excerpt from wardyn-ebpf — the LSM file_open enforcement path" width="100%"/>
</div>

<br/>

### Focus

**Runtime containment** — kernel-level wardens and sealed execution environments for autonomous AI agents, enforced below the process rather than negotiated with it.

**Verifiable privacy** — transparent L7 data-masking proxies and zero-knowledge proofs, so a result can be trusted without trusting the machine that produced it.

**Decentralised transport** — offline disaster-communication nodes and enterprise API gateways coordinated by gossip protocols and CRDTs, built to survive the network being wrong.

<br/>

<div align="center">
<img src="assets/stack.svg" alt="Component schedule — Rust, Python, Go, Kotlin, eBPF, Kubernetes, CRDT, Ed25519, zkVM, PostgreSQL" width="100%"/>
</div>

Rust for the parts that must not fail, Python and Go for the parts that must move quickly. Everything ships containerised and orchestrated — Docker and Kubernetes, minimal egress, fault tolerance assumed rather than added later. Working is the floor; deterministic and stable at the edge of the machine's capacity is the bar.

<br/>

<div align="center">
<img src="assets/register.svg" alt="Project register — ten systems, one open source, nine private" width="100%"/>
</div>

From explainable-AI middleware to UDP-based WAN file transfer, the through-line is the same: push the boundary where network optimisation meets machine learning, and keep latency and trust on the right side of it.

<br/>

<div align="center">
<img src="assets/upstream.svg" alt="Upstream record — eight patches merged into NASA F´, NASA spacewasm and CERN CernVM-FS" width="100%"/>
</div>

Eight patches merged into code other people's missions depend on: build-system correctness in **F´**, the NASA flight software framework flown on the Ingenuity Mars helicopter; host-interface and build fixes in **spacewasm**, NASA's flight-compliant WebAssembly interpreter; and a toolchain-discovery fix in **CernVM-FS**, the filesystem CERN uses to distribute LHC experiment software to computing sites worldwide. Reading an unfamiliar build system until the failure is obvious is the same work as reading a kernel path — only with a stricter review queue. More are in review.

**[nasa/fprime](https://github.com/nasa/fprime)** · [#5590](https://github.com/nasa/fprime/pull/5590) · [#5576](https://github.com/nasa/fprime/pull/5576) · [#5571](https://github.com/nasa/fprime/pull/5571) · [#5559](https://github.com/nasa/fprime/pull/5559)<br/>
**[nasa/spacewasm](https://github.com/nasa/spacewasm)** · [#154](https://github.com/nasa/spacewasm/pull/154) · [#153](https://github.com/nasa/spacewasm/pull/153) · [#152](https://github.com/nasa/spacewasm/pull/152)<br/>
**[cvmfs/cvmfs](https://github.com/cvmfs/cvmfs)** · [#4392](https://github.com/cvmfs/cvmfs/pull/4392)

<br/>

I'm open to systems and infrastructure work — Rust services, kernel and network-level tooling, distributed architecture, and security engineering. If you need help or know someone who does, I'd appreciate an introduction.

`kadir.can.yildirm@gmail.com`

<br/>

<div align="center">

<img src="https://visitor-badge.laobi.icu/badge?page_id=kadircanyildirm-crypto.readme&title=PROFILE%20VIEWS&left_color=%231D1219&right_color=%23C81E45" alt="Profile views" height="30"/>

<img src="assets/footer.svg" alt="Drawing set KC-001 to KC-050 · revision 2026.08 · Anadolu University" width="100%"/>

</div>
