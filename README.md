# CO-WEEK Semiconductor Industry Insights

2026년 6월 29일~7월 3일 평창 알펜시아 리조트에서 열린 **제5회 CO-WEEK ACADEMY**에 4박 5일간 참여하고, 서울대학교 2026학년도 하계 계절학기 **(공유)반도체산업이해** 교과목과 연계해 수행한 산업·기술 탐색 프로젝트입니다.

CO-WEEK 기간 동안 10개 강의를 선택해 수강하면서 **반도체 소재 → 트랜지스터 → CMOS 회로 → HBM/첨단패키징 → AI → 양자컴퓨팅**으로 이어지는 기술 스택을 폭넓게 탐색했습니다.

이후 가장 인상 깊었던 **「HBM에서 양자컴퓨팅까지: 병렬 처리의 원리」** 강의를 바탕으로, CPU–GPU–HBM–Quantum으로 이어지는 계산 패러다임과 classical–quantum hybrid architecture의 실효성을 소자·공정 관점에서 비판적으로 분석하는 2페이지 심화 보고서를 작성했습니다.

> This repository is a learning-and-industry-insight portfolio. It does not claim original device fabrication, simulation, or experimental results.

---

## Program at a Glance

| Item | Details |
|---|---|
| Program | 제5회 CO-WEEK ACADEMY |
| Period | 2026.06.29–07.03 |
| Venue | 강원도 평창 알펜시아 리조트 |
| Organizer | 교육부 · 한국연구재단 / 첨단분야 혁신융합대학 사업단 협의회 |
| Course | 서울대학교 (공유)반도체산업이해 |
| Course type | 2026 하계 계절학기 · 전공선택 · 2학점 |
| Course format | 1주 오프라인 CO-WEEK + 1주 온라인 단기집중강좌 |
| CO-WEEK completion criterion | 10개 이상 수료증, 이 중 차세대반도체 강의 6개 이상 |
| My focus | Semiconductor technology stack from device to computing architecture |

Official program:
- https://academy.cossnet.com/coweek/intro
- https://www.disu.ac.kr/community/notice?bbsidx=8662&md=v

---

## 10 Lectures I Selected

| # | Lecture |
|---:|---|
| 1 | 양자컴퓨터와 반도체 기술 |
| 2 | 반도체 소재의 이해와 트랜지스터 제작 기초 |
| 3 | HBM에서 양자컴퓨팅까지 |
| 4 | 미래자동차 시대의 기업가 정신 |
| 5 | 실리콘 나노입자 |
| 6 | 트랜지스터 동작원리 |
| 7 | 인공지능, 반도체를 만나다 |
| 8 | 반도체 임팩트 |
| 9 | CMOS 논리회로 입문 |
| 10 | 양자역학 비교적 쉽게 이해하기 |

The selected lectures intentionally span different abstraction levels rather than staying within one narrow topic.

---

## My Learning Map

```text
Materials
  ↓
Transistor fabrication / device physics
  ↓
CMOS logic
  ↓
Memory bandwidth / HBM / advanced packaging
  ↓
AI acceleration
  ↓
Quantum computing
  ↓
Hybrid / heterogeneous computing
```

This made it possible to connect process engineering with the larger question of **where future computing bottlenecks actually move after transistor scaling alone is no longer enough**.

---

## Deep-Dive Reflection

### From von Neumann bottleneck to GPU + HBM

The report starts from the physical separation between processor and memory in conventional computing.

As AI workloads scale:

- CPU-centric execution becomes insufficient for highly parallel workloads
- GPU parallelism increases throughput
- HBM reduces the memory-bandwidth bottleneck
- TSV-based stacking and advanced packaging become essential to keep data physically close to compute

The key insight is that performance improvement is no longer only a transistor problem. **Memory architecture and packaging are now part of compute performance.**

### From classical computing to quantum acceleration

The lecture introduced quantum computing as a candidate for problems that remain difficult for classical systems.

Rather than assuming that quantum computers replace CPUs/GPUs, the report focused on a more realistic **hybrid model**:

```text
CPU / GPU / HPC
      +
Quantum accelerator
      ↓
problem-specific heterogeneous computing
```

### My Critical Question

My report then asked:

> Even if quantum algorithms offer an advantage, can a fragile quantum system be integrated with deterministic CMOS electronics without excessive interface, control, conversion, and error-correction overhead?

This was motivated by previous TCAD experience, where device performance changed significantly with nanoscale process parameters such as implantation dose, energy, and junction profile.

The reflection therefore moved the discussion from a system-level architecture diagram back down to **device physics, materials, process control, and interface engineering**.

---

## Updated Industry Context

### Quantum + HPC is becoming an explicit architecture direction

IBM's 2026 quantum roadmap describes quantum advantage in an integrated system using quantum hardware together with HPC, and its 2026 reference architecture explicitly positions QPUs alongside CPUs and GPUs.

This supports the lecture's central idea that near-term quantum computing is more likely to appear as **heterogeneous acceleration** than as a complete replacement for classical semiconductor systems.

Sources:
- https://www.ibm.com/roadmaps/quantum/2026/
- https://newsroom.ibm.com/2026-03-12-ibm-releases-a-new-blueprint-for-quantum-centric-supercomputing

### Neuromorphic computing is another complementary path

My original report presented neuromorphic devices as a possible alternative response to the limits of conventional computing.

A more careful current interpretation is:

- quantum computing targets selected problem classes using fundamentally different computational resources
- neuromorphic computing targets energy-efficient sensing / inference / brain-inspired workloads
- advanced CMOS, HBM, packaging, and accelerators continue to improve classical computing

These approaches should be viewed as **coexisting computing paradigms**, not as a simple winner-takes-all replacement sequence.

Recent neuromorphic literature continues to emphasize low-power, parallel, hardware-native processing and memristive devices that combine memory and computation.

Sources:
- https://www.nature.com/articles/s44287-025-00235-w
- https://www.nature.com/articles/s44287-025-00229-8

---

## What I Learned

### 1. Semiconductor performance is a stack problem

Transistor scaling alone does not determine system performance.

The relevant stack now includes:

- device electrostatics
- circuit architecture
- memory bandwidth
- interconnect
- advanced packaging
- accelerator architecture
- software / workload mapping

### 2. HBM is a process and packaging problem as much as a memory problem

AI compute exposed data movement as a system bottleneck.

HBM therefore connects:

- DRAM process
- wafer thinning
- TSV
- bonding
- thermal design
- yield
- package integration

This was particularly relevant to my interest in semiconductor process / manufacturing engineering.

### 3. Future computing still depends on physical interfaces

Even a high-level concept such as quantum-classical hybrid computing ultimately depends on:

- signal conversion
- control electronics
- cryogenic / thermal interface
- device reliability
- interconnect latency
- materials stability

System architecture cannot escape device physics.

### 4. Broad lectures became more useful when connected back to one engineering axis

The ten lectures covered very different topics, but the common question became:

> **What physical bottleneck is each technology trying to remove?**

This turned the CO-WEEK experience from a list of lectures into a technology map.

---

## Read the Project

| Page | Description |
|---|---|
| [Project Page](./index.html) | 전체 학습 흐름 요약 |
| [Navigation](./guide/00_navigation.md) | 전체 문서 안내 |
| [Program Context](./guide/01_program_context.md) | CO-WEEK 및 교과목 구조 |
| [Lecture Learning Map](./guide/02_lecture_learning_map.md) | 10개 강의를 기술 스택으로 재구성 |
| [HBM & Parallel Computing](./guide/03_hbm_parallel_computing.md) | CPU–GPU–HBM 관점 |
| [Quantum Hybrid Computing](./guide/04_quantum_hybrid.md) | classical–quantum hybrid model |
| [Device-Level Reflection](./guide/05_device_level_reflection.md) | 소자·공정 관점의 비판적 고찰 |
| [Industry Expansion](./guide/06_industry_research.md) | IBM·neuromorphic 추가 조사 |
| [Career Takeaways](./guide/07_career_takeaways.md) | 공정/양산 관점에서 얻은 의미 |
| [Evidence Scope](./guide/08_evidence_scope.md) | 원본 보고서와 추가 조사 구분 |
| [References](./references/README.md) | 공식 프로그램·외부 조사 출처 |
| [Report Scope](./report/README.md) | 원본 2페이지 보고서 설명 |

---

## Structured Data

- [lecture_learning_map.csv](./results/lecture_learning_map.csv)
- [computing_stack.csv](./results/computing_stack.csv)
- [reflection_matrix.csv](./results/reflection_matrix.csv)

These are portfolio-organized learning records, not experimental datasets.

---

## Repository Structure

```text
CO-WEEK-Semiconductor-Industry-Insights/
├── README.md
├── index.html
├── index.md
├── _config.yml
├── assets/
├── guide/
├── results/
├── study/
├── references/
├── appendix/
├── source/
└── report/
```

---

## Scope

This repository separates three evidence levels:

1. **Personal experience** — the 10 lectures selected and the submitted reflection report
2. **Official program information** — CO-WEEK / course operation details
3. **Additional research** — current external context added after the course

The additional research is used to expand the portfolio interpretation, not to retroactively claim that it was part of the original submitted assignment.

---

[← Back to Subin Joo's GitHub Portfolio](https://github.com/soybeanmilk0514-jpg)
