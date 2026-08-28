<div align="center">

# Yang Jiseop | 양지섭

### Game Client Programmer

**Unity/C# 프로젝트 경험을 기반으로 Unreal Engine 5/C++ 역량을 확장 중인 신입 게임 클라이언트 개발자입니다.**

   <!-- POKEREPO:START -->
   <!-- POKEREPO:END -->

4인 팀 `KrameLife`에서 프로젝트 관리와 클라이언트 통합을 담당했습니다.<br>기능을 구현하는 데서 그치지 않고, 플레이 흐름과 팀의 작업 기준까지 연결합니다.

[Representative Project: KrameLife](https://github.com/Femur-0607/KrameLife-Portfolio) · [KrameLife Demo](https://youtu.be/ArTEC_peleQ) · [MiniDriller Demo](https://youtu.be/efCUcJviVkE)

</div>

---

## About Me

- **입력 → 상태 → UI → 데이터 → 저장**이 하나의 플레이 흐름으로 이어지도록 구조화합니다.
- 버그는 **재현 → 원인 분석 → 구조 수정 → 검증** 순서로 해결하고, 문제와 의사결정 과정을 다시 확인할 수 있게 기록합니다.
- 기능 범위와 완료 기준, 진행 상황을 문서화해 팀원이 같은 기준으로 작업할 수 있도록 돕습니다.

## Tech Stack

**주력** &nbsp; ![Unity](https://img.shields.io/badge/Unity-222222?style=flat-square&logo=unity&logoColor=white) ![C#](https://img.shields.io/badge/C%23-68217A?style=flat-square&logo=csharp&logoColor=white)

**프로젝트 경험 · 확장 중** &nbsp; ![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-0E1128?style=flat-square&logo=unrealengine&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) `Meta XR` `Paper2D / PaperZD`

**협업** &nbsp; ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)

**구현 경험** &nbsp; `Gameplay Logic` `UI` `Data-driven Design` `Save/Load` `Object Pooling` `FSM` `Addressables` `VR Interaction`

## Featured Projects

### KrameLife - 협업 중심 2D 경영 RPG

[![KrameLife Demo](https://img.youtube.com/vi/ArTEC_peleQ/hqdefault.jpg)](https://youtu.be/ArTEC_peleQ)

`Unity 6.3 LTS` `C#` `4인 팀` `프로젝트 관리 · 클라이언트 통합`

- 아이템 데이터가 Inspector와 개별 ScriptableObject에 흩어진 문제를 해결하기 위해 `CSV → ScriptableObject → GameDatabase` 파이프라인과 일괄 검증을 구성했습니다.
- 공통 ID 규칙, Addressables 기반 아이콘 로딩, `GameContext` 상태 접근으로 팀 기능이 같은 데이터 기준을 사용하도록 연결했습니다.
- 기능 범위·우선순위·담당·완료 기준과 회의 결정을 문서화하고, 팀원 기능을 메인 플레이 흐름에 통합했습니다.

[Repository](https://github.com/Femur-0607/KrameLife-Portfolio) · [Demo Video](https://youtu.be/ArTEC_peleQ)

### MiniDriller - 논리 좌표로 규칙을 안정화한 2D 채굴 액션

[![MiniDriller Demo](https://img.youtube.com/vi/efCUcJviVkE/hqdefault.jpg)](https://youtu.be/efCUcJviVkE)

`Unreal Engine 5.6.1` `C++` `Paper2D / PaperZD` `1인 개발` `14일`

- 물리 충돌 순서에 따라 블록이 멈추거나 겹치는 문제를 재현했습니다.
- `TMap<FIntPoint, ABlock*>` GridMap에서 논리 좌표를 먼저 확정하도록 구조를 바꿔 낙하와 Match-4 판정을 일관되게 처리했습니다.
- Flood Fill, 타입별 Object Pooling을 구현하고 반복자 무효화·이중 반납 문제까지 검증했습니다.

[Repository](https://github.com/Femur-0607/MiniDriller-Portfolio) · [Demo Video](https://youtu.be/efCUcJviVkE) · [Dev Logs](https://github.com/Femur-0607/MiniDriller-Portfolio/tree/main/Docs/Notion/dev-logs) · [Troubleshooting](https://github.com/Femur-0607/MiniDriller-Portfolio/blob/main/Docs/Notion/troubleshooting.md)

### Castle Guardian VR - 입력과 피드백을 연결한 VR 디펜스

[![Castle Guardian VR Demo](https://img.youtube.com/vi/KxXcOsSTjww/hqdefault.jpg)](https://youtu.be/KxXcOsSTjww)

`Unity` `C#` `Meta XR SDK` `1인 개발` `8주`

- 낯선 VR 개발 환경에서 Meta·Unity 공식 문서를 기준으로 입력과 상호작용을 작은 단위로 구현하고 반복 검증했습니다.
- 활·투사체, 웨이브·적 AI, 타워 시스템의 책임을 나누고 ScriptableObject로 데이터를 분리했습니다.
- 적, 투사체, 파티클, 오디오에 Object Pooling을 적용해 하나의 플레이 가능한 디펜스 흐름으로 연결했습니다.

[Repository](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio) · [Demo Video](https://youtu.be/KxXcOsSTjww)

## Collaboration & Communication

| 협업 기준 | 실행과 근거 |
| --- | --- |
| 같은 기준으로 시작 | 기능 범위, 공통 ID·데이터 규칙, 완료 기준과 검증 절차를 먼저 정리합니다. [Team Development Rules](https://github.com/Femur-0607/Project-CoreLoop/blob/master/docs/team-rules.md) |
| 진행과 결정을 공유 | 작업 보드·회의 기록·개발일지에 진행 상태, 결정 이유, 남은 위험을 남깁니다. [Development Notes](https://github.com/Femur-0607/MiniDriller-Portfolio/blob/main/Docs/Notion/README.md) |
| 메인 흐름에서 통합 | 팀원 기능을 공통 데이터와 플레이 흐름에 연결하고 함께 검증합니다. [KrameLife Repository](https://github.com/Femur-0607/KrameLife-Portfolio) · [Demo](https://youtu.be/ArTEC_peleQ) |

라이브 게임 CS 경험을 바탕으로 사용자 이슈를 재현 가능한 형태로 정리하고, 상대가 이해하기 쉬운 언어로 전달합니다.

## Growth & Records

[DunLegacy](https://github.com/Femur-0607/DunLegacy-Portfolio)의 폭넓은 기능 구현 → [Castle Guardian VR](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio)의 책임 분리 → [MiniDriller](https://github.com/Femur-0607/MiniDriller-Portfolio)의 논리 좌표 중심 구조 → [KrameLife](https://github.com/Femur-0607/KrameLife-Portfolio)의 팀 공통 데이터·협업 기준으로 프로젝트마다 설계 범위를 확장해 왔습니다.

C++ 학습 과정도 [MissingDiamond 커밋 기록](https://github.com/Femur-0607/MissingDiamond/commits/master/)에 작은 리팩터링 단위로 남겨 변화의 이유를 확인할 수 있게 했습니다.

