# 03. HBM & Parallel Computing

## The Bottleneck Moved

심화 보고서의 출발점은 von Neumann architecture의 processor–memory separation이다.

연산 장치의 성능이 빨라져도 데이터가 제때 공급되지 않으면 전체 system throughput은 제한된다.

AI workload에서는 이 문제가 더 크게 드러난다.

## CPU → GPU

CPU는 general-purpose serial / lightly parallel workloads에 강하지만, deep learning의 matrix-style operations에는 대규모 parallel processing이 유리하다.

GPU는 많은 compute cores를 통해 이 문제를 해결한다.

하지만 GPU 수가 늘어나면 다음 bottleneck은 **memory bandwidth와 data movement**로 이동한다.

## Why HBM Matters

HBM은 여러 DRAM die를 적층하고 TSV와 advanced packaging을 이용해 compute와 memory 사이의 대역폭을 높이는 방향이다.

이 프로젝트에서 중요하게 느낀 점은 HBM이 단순한 memory product가 아니라 다음 공정·제조기술의 집합이라는 것이다.

- DRAM process
- wafer thinning
- TSV formation
- bonding
- package integration
- thermal management
- yield control

## Process-Engineering Perspective

AI 시대의 성능 경쟁은 transistor scaling만으로 설명하기 어렵다.

소자 성능이 좋아져도:

- memory bandwidth가 부족하거나
- package thermal path가 나쁘거나
- bonding yield가 낮으면

제품 수준의 성능과 생산성이 제한된다.

따라서 공정 엔지니어링 역시 system performance의 일부라고 이해하게 됐다.
