# 05. Device-Level Reflection

## My Report's Critical Question

원본 심화 보고서는 system architecture의 가능성을 그대로 받아들이기보다 다음 의문을 제기했다.

> fragile quantum state와 deterministic CMOS electronics 사이의 interface가 실제 system advantage를 유지할 수 있는가?

보고서에서는 quantum state의 decoherence와 classical signal conversion / synchronization overhead를 문제로 보았다.

## Why I Asked This Question

이전 TCAD 프로젝트에서 implantation dose, energy, junction profile처럼 nanoscale parameter가 transistor leakage와 switching behavior를 크게 바꾸는 것을 경험했다.

그 경험 때문에, quantum-classical architecture 역시 block diagram만으로는 충분하지 않고 실제 interface와 device-level implementation을 봐야 한다고 생각했다.

## Refined Interpretation

원본 보고서에서는 interface overhead가 quantum advantage를 상쇄할 수 있다는 강한 문제의식을 제시했다.

이 포트폴리오에서는 이를 확정적 결론이 아니라 **engineering question**으로 재정리한다.

검토해야 할 항목:
- QPU control and readout
- cryogenic CMOS
- conversion / communication latency
- error-correction overhead
- physical interconnect
- materials and device reliability

## Process Insight

High-level computing architecture도 최종적으로는 physical device와 process technology 위에서 구현된다.

따라서 미래 computing을 이해할 때 software / algorithm뿐 아니라 **device–material–process interface**까지 같이 봐야 한다는 점이 가장 큰 학습이었다.
