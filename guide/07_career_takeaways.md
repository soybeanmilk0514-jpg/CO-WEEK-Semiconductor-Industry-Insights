# 07. Career Takeaways — Process / Manufacturing View

## 1. Product Performance Depends on Manufacturing

HBM을 공부하면서 high-level AI performance가 결국 다음 제조 요소에 의해 제한될 수 있음을 이해했다.

- TSV process
- wafer thinning
- bonding accuracy
- defect control
- thermal process
- package yield

따라서 양산기술 / 공정기술은 단순히 recipe를 유지하는 직무가 아니라 product architecture의 요구를 실제 wafer/package 위에 구현하는 역할과 연결된다.

## 2. Cross-Layer Communication Matters

소자 엔지니어는 architecture를, architecture engineer는 manufacturing constraint를 완전히 무시할 수 없다.

예:
- HBM bandwidth target ↔ TSV / bonding / thermal constraint
- low-voltage logic ↔ leakage / variation constraint
- quantum control ↔ cryogenic electronics / material constraint

## 3. Broad Learning Helps Identify the Real Bottleneck

CO-WEEK에서 서로 다른 강의를 들은 가장 큰 장점은 기술명을 많이 알게 된 것보다, 문제를 봤을 때 “현재 bottleneck이 어디인가?”를 먼저 생각하게 된 점이다.

## 4. My Career Connection

이 경험은 반도체 공정 / 양산 엔지니어가:

- device physics
- integration
- equipment
- yield
- reliability
- package interaction

을 함께 이해해야 한다는 인식을 강화했다.

특히 앞으로 프로젝트를 볼 때도 “성능이 좋아졌다”에서 끝나지 않고 **어떤 공정변수가 제품 성능과 수율을 동시에 제한하는가**를 확인하는 관점을 유지하고자 한다.
