# 04. Quantum–Classical Hybrid Computing

## Lecture-Level Idea

심화 보고서에서 다룬 핵심 모델은 classical computer와 quantum computer를 완전히 대체 관계로 보는 것이 아니라 역할을 나누는 것이다.

```text
Classical CPU / GPU / HPC
          +
Quantum accelerator
          ↓
Problem-specific heterogeneous computing
```

범용 orchestration, data preparation, control, and conventional workloads는 classical system이 맡고, quantum advantage가 기대되는 특정 subproblem을 quantum processor가 담당하는 그림이다.

## Current Industry Context Added After the Course

IBM의 2026 quantum roadmap은 quantum hardware를 HPC와 통합해 quantum-classical workload를 실행하는 방향을 명시하고 있다.

또한 IBM은 2026년 quantum-centric supercomputing reference architecture에서 QPU가 CPU/GPU와 함께 동작하는 구조를 제시했다.

따라서 강의에서 제시된 hybrid model은 단순한 미래 상상이 아니라 실제 산업 roadmap에서 다뤄지는 architecture direction과 연결된다.

## Important Caution

이것이 곧 quantum computer가 모든 classical workload보다 빠르다는 뜻은 아니다.

실제 시스템에는:

- error correction
- control electronics
- cryogenic infrastructure
- job orchestration
- classical pre/post-processing
- interconnect / latency

등이 함께 필요하다.

Hybrid system의 가치는 workload-specific하게 판단해야 한다.
