# 06. Additional Industry Research

이 문서는 원본 제출 보고서 이후 포트폴리오를 만들면서 추가 조사한 내용이다.

## 1. IBM: Quantum + HPC Integration

IBM의 2026 roadmap은 quantum advantage를 quantum computer와 HPC를 함께 사용하는 integrated system에서 탐색하는 방향을 제시한다.

또한 CPU, GPU, QPU가 함께 동작하도록 orchestration하는 quantum-centric supercomputing reference architecture를 공개했다.

이 흐름은 near-term quantum computing을 **standalone replacement**보다 **heterogeneous accelerator**로 보는 해석을 뒷받침한다.

## 2. Neuromorphic Computing

원본 보고서에서는 memristor / neuromorphic device를 quantum computing의 대안적 경로로 제시했다.

최근 literature를 추가로 검토하면, 더 정확한 표현은 “대체재 하나”보다 **서로 다른 workload를 겨냥하는 complementary paradigm**에 가깝다.

Neuromorphic computing이 집중하는 문제:
- low-power sensing
- event-driven processing
- memory / compute co-location
- brain-inspired parallelism

Memristive devices는 memory와 processing을 한 소자에서 수행하는 방향으로 연구되고 있다.

## 3. A Better Technology Map

미래 computing을 단일 순서로 보는 대신 다음처럼 보는 것이 더 적절하다.

| Paradigm | Main target |
|---|---|
| Advanced CMOS | general-purpose efficient computing |
| GPU + HBM | data-parallel AI / HPC |
| Neuromorphic | event-driven / energy-efficient inference and sensing |
| Quantum | selected problems with quantum algorithmic advantage |
| Advanced packaging | heterogeneous integration across all of the above |

## Conclusion

미래 semiconductor 산업의 경쟁은 하나의 device가 모든 것을 대체하는 구조보다, 여러 compute / memory / package technology가 **heterogeneously integrated**되는 방향으로 이해하는 것이 더 현실적이다.
