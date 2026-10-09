<div align="center">

# Yang Jiseop | 양지섭

### Game Client Programmer

**Unity/C# 프로젝트 경험을 기반으로 Unreal Engine 5/C++ 역량을 확장 중인 신입 게임 클라이언트 개발자입니다.**

Unity 팀 프로젝트의 관리·통합부터 Unreal C++ 1인 개발, 개발 도구 제작까지 경험했습니다.<br>기능 구현에서 그치지 않고 플레이 흐름, 팀의 작업 기준, 개발 환경까지 연결합니다.

**팀 프로젝트** [KrameLife](https://github.com/Femur-0607/KrameLife-Portfolio) ([Demo](https://youtu.be/ArTEC_peleQ)) &nbsp;·&nbsp; **1인 개발** [MiniDriller](https://github.com/Femur-0607/MiniDriller-Portfolio) ([Demo](https://youtu.be/efCUcJviVkE)) &nbsp;·&nbsp; **개발 도구** [handback](https://github.com/Femur-0607/handback)

</div>

---

## About Me

- **플레이 흐름 단위로 완성합니다.** 입력 → 상태 → UI → 데이터 → 저장이 끊기지 않게 구조화하고, 메인 흐름에서 동작해야 완료로 봅니다.
- **버그는 구조에서 고칩니다.** 재현 → 원인 분석 → 구조 수정 → 검증 순서로 해결하고 과정을 기록합니다. [예시](https://github.com/Femur-0607/MiniDriller-Portfolio/blob/main/Docs/Notion/troubleshooting.md)
- **팀이 같은 기준으로 일하게 합니다.** 기능 범위, 공통 ID·데이터 규칙, 완료 기준을 먼저 문서로 맞춥니다. [팀 개발 규칙](https://github.com/Femur-0607/KrameLife-Portfolio/blob/main/Docs/team-rules.md)
- **사용자 관점으로 전달합니다.** 라이브 게임 CS 경험으로 사용자 이슈를 재현 가능한 형태로 정리해 쉬운 언어로 전달합니다.

## Tech Stack

**주력** &nbsp; ![Unity](https://img.shields.io/badge/Unity-222222?style=flat-square&logo=unity&logoColor=white) ![C#](https://img.shields.io/badge/C%23-68217A?style=flat-square&logo=csharp&logoColor=white)

**프로젝트 경험 · 확장 중** &nbsp; ![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-0E1128?style=flat-square&logo=unrealengine&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) `Meta XR` `Paper2D / PaperZD`

**도구 · 협업** &nbsp; ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)

## Featured Projects

### KrameLife - 팀 기능을 하나의 데이터 기준으로 묶은 2D 경영 RPG

[![KrameLife Demo](https://img.youtube.com/vi/ArTEC_peleQ/hqdefault.jpg)](https://youtu.be/ArTEC_peleQ)

`Unity 6.3 LTS` `C#` `4인 팀` `Core 공통 토대 · 데이터 파이프라인 · 클라이언트 통합 · 프로젝트 관리`

- **데이터 불일치 제거:** 흩어진 아이템 데이터를 `CSV → 검증 → ScriptableObject → GameDatabase`로 일원화하고, ID 중복·필수값·아이콘 주소를 임포트 전에 검사했습니다.
- **기능을 붙이기 쉬운 저장 구조:** `ISaveParticipant` 단위 JSON Save/Load로 도감·시간·가게·평판을 하나의 저장 흐름에 연결했습니다.
- **팀 기능 통합:** `GameContext`, 이벤트 채널, Additive Scene Flow로 팀원 기능을 메인 플레이 흐름에 연결했습니다.

[Repository](https://github.com/Femur-0607/KrameLife-Portfolio) · [Demo](https://youtu.be/ArTEC_peleQ) · 코드: [GameDatabase](https://github.com/Femur-0607/KrameLife-Portfolio/blob/main/Assets/_Project/01.Scripts/01.Core/Databases/GameDatabase.cs) · [SaveManager](https://github.com/Femur-0607/KrameLife-Portfolio/blob/main/Assets/_Project/01.Scripts/01.Core/Save/SaveManager.cs) · [SceneFlowManager](https://github.com/Femur-0607/KrameLife-Portfolio/blob/main/Assets/_Project/01.Scripts/01.Core/SceneFlow/Persistent/SceneFlowManager.cs)

### MiniDriller - 논리 좌표로 규칙을 안정화한 2D 채굴 액션

[![MiniDriller Demo](https://img.youtube.com/vi/efCUcJviVkE/hqdefault.jpg)](https://youtu.be/efCUcJviVkE)

`Unreal Engine 5.6.1` `C++` `Paper2D / PaperZD` `1인 개발` `14일`

- **블록 멈춤·겹침 해결:** 물리 충돌 순서에 의존하던 판정을 `TMap<FIntPoint, ABlock*>` GridMap의 논리 좌표 우선 구조로 바꿔 낙하와 Match-4 판정을 일관되게 만들었습니다.
- **블록 재사용 안정화:** 타입별 Object Pooling과 Flood Fill을 구현하고, 반복자 무효화·이중 반납 문제를 검증했습니다.

[Repository](https://github.com/Femur-0607/MiniDriller-Portfolio) · [Demo](https://youtu.be/efCUcJviVkE) · [Troubleshooting](https://github.com/Femur-0607/MiniDriller-Portfolio/blob/main/Docs/Notion/troubleshooting.md) · 코드: [MapManager](https://github.com/Femur-0607/MiniDriller-Portfolio/blob/main/Source/MiniDriller/Private/MapManager.cpp)

### Castle Guardian VR - 처음 다룬 VR 입력을 플레이 흐름으로 연결한 디펜스

[![Castle Guardian VR Demo](https://img.youtube.com/vi/KxXcOsSTjww/hqdefault.jpg)](https://youtu.be/KxXcOsSTjww)

`Unity` `C#` `Meta XR SDK` `1인 개발` `8주`

- **낯선 환경을 작은 단위로 검증:** Meta·Unity 공식 문서를 기준으로 활 입력과 상호작용을 단계별로 구현하고 반복 검증했습니다.
- **시스템별 책임 분리:** 활·투사체, 웨이브·적 AI, 타워를 나누고 ScriptableObject로 데이터를, Object Pooling으로 적·투사체·파티클·오디오 생성을 분리했습니다.

[Repository](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio) · [Demo](https://youtu.be/KxXcOsSTjww) · 코드: [ArrowShooter](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio/blob/main/Assets/06.Scripts/02.BowArrow/ArrowShooter.cs) · [WaveManager](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio/blob/main/Assets/06.Scripts/01.WaveSystem/WaveManager.cs)

## Side Project

### handback - 코딩 에이전트 앱 사이의 작업 전달 도구

<a href="https://github.com/Femur-0607/handback"><img src="https://raw.githubusercontent.com/Femur-0607/handback/main/docs/assets/handback-logo.png" alt="handback" width="320"></a>

`Python` `표준 라이브러리만 사용` `1인 개발` `PyPI 공개`

- **작업 전달과 결과 회수:** Claude 대화(Lead)가 Codex·Antigravity 워커 대화에 작업을 넘기고, 결과를 로컬 inbox로 받아 검토·확인(ACK)합니다.
- **중단돼도 이어받기:** 요청별 식별자와 디스크 저장으로 대화 종료·타임아웃 뒤에도 중복 제출 없이 복구합니다.
- **설치 한 줄, 추가 의존성 없음:** 앱 실행·파일 감시·JSON 처리 위주라 Python 표준 라이브러리만으로 구현해, 에이전트 앱의 훅·스킬에서 바로 호출됩니다.

[Repository](https://github.com/Femur-0607/handback) · [PyPI](https://pypi.org/project/handback/) · [한국어 사용 설명서](https://github.com/Femur-0607/handback/blob/main/docs/usage.ko.md)

## Growth

[DunLegacy](https://github.com/Femur-0607/DunLegacy-Portfolio)(폭넓은 기능 구현) → [Castle Guardian VR](https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio)(책임 분리) → [MiniDriller](https://github.com/Femur-0607/MiniDriller-Portfolio)(논리 좌표 중심 구조) → [KrameLife](https://github.com/Femur-0607/KrameLife-Portfolio)(팀 공통 데이터·협업 기준) 순으로 설계 범위를 넓혀 왔습니다. C++ 학습은 [MissingDiamond 커밋 기록](https://github.com/Femur-0607/MissingDiamond/commits/master/)에 작은 리팩터링 단위로 남겼습니다.

---

<div align="center">

<!-- POKEREPO:START -->
<table>
<tr>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=543" title="Venipede in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/543.gif" width="64" height="45" alt="venipede"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=846" title="Arrokuda in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/846.png" width="64" height="64" alt="arrokuda"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=582" title="Vanillite in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/582.gif" width="64" height="52" alt="vanillite"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=16" title="Pidgey in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/16.gif" width="56" height="64" alt="pidgey"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=21" title="Spearow in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/21.gif" width="53" height="64" alt="spearow"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=843" title="Silicobra in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/843.png" width="64" height="64" alt="silicobra"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=824" title="Blipbug in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/824.png" width="64" height="64" alt="blipbug"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=74" title="Geodude in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/74.gif" width="64" height="47" alt="geodude"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=333" title="Swablu in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/333.gif" width="64" height="43" alt="swablu"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=572" title="Minccino in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/572.gif" width="64" height="55" alt="minccino"></a></td>
<td align="center" valign="bottom" width="80" height="64"><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=524" title="Roggenrola in the Dex"><img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/versions/generation-v/black-white/animated/524.gif" width="39" height="64" alt="roggenrola"></a></td>
</tr>
<tr>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=543"><b>Venipede</b></a><br><sub>Lv.17</sub><br><sub><a href="https://github.com/Femur-0607/Femur-0607" title="Femur-0607/Femur-0607">Femur-0607</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=846"><b>Arrokuda</b></a><br><sub>Lv.16</sub><br><sub><a href="https://github.com/Femur-0607/handback" title="Femur-0607/handback">handback</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=582"><b>Vanillite</b></a><br><sub>Lv.14</sub><br><sub><a href="https://github.com/Femur-0607/MissingDiamond" title="Femur-0607/MissingDiamond">MissingDiam…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=16"><b>Pidgey</b></a><br><sub>Lv.9</sub><br><sub><a href="https://github.com/Femur-0607/MiniDriller-Portfolio" title="Femur-0607/MiniDriller-Portfolio">MiniDriller…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=21"><b>Spearow</b></a><br><sub>Lv.7</sub><br><sub><a href="https://github.com/Femur-0607/KrameLife-Portfolio" title="Femur-0607/KrameLife-Portfolio">KrameLife-P…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=843"><b>Silicobra</b></a><br><sub>Lv.7</sub><br><sub><a href="https://github.com/Femur-0607/Project-CoreLoop" title="Femur-0607/Project-CoreLoop">Project-Cor…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=824"><b>Blipbug</b></a><br><sub>Lv.7</sub><br><sub><a href="https://github.com/Femur-0607/speak-flow" title="Femur-0607/speak-flow">speak-flow</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=74"><b>Geodude</b></a><br><sub>Lv.7</sub><br><sub><a href="https://github.com/Femur-0607/CodeTest" title="Femur-0607/CodeTest">CodeTest</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=333"><b>Swablu</b></a><br><sub>Lv.6</sub><br><sub><a href="https://github.com/Femur-0607/DunLegacy-Portfolio" title="Femur-0607/DunLegacy-Portfolio">DunLegacy-P…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=572"><b>Minccino</b></a><br><sub>Lv.6</sub><br><sub><a href="https://github.com/Femur-0607/Castle-Guardian-VR-Portfolio" title="Femur-0607/Castle-Guardian-VR-Portfolio">Castle-Guar…</a></sub></td>
<td align="center" valign="top" nowrap><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607&m=524"><b>Roggenrola</b></a><br><sub>Lv.1 · parked</sub><br><sub><a href="https://github.com/Femur-0607/KrameLife" title="Femur-0607/KrameLife">KrameLife</a></sub></td>
</tr>
</table>

<sub><a href="https://wantaekchoi.github.io/pokerepo/?u=Femur-0607">Femur-0607's Dex</a></sub>
<!-- POKEREPO:END -->

</div>
