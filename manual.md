# Tangle-Ops User Manual (KR/EN)

## 개요
Tangle-Ops는 격자형 퍼즐 게임입니다. 녹색 유닛을 움직이면 빨간 유닛이
반대 방향으로 움직입니다. 두 유닛을 동시에 각 목표 지점에 올려야 합니다.

## 승리 조건
- 녹색 유닛이 녹색 목표 프레임에 도달
- 빨간 유닛이 빨간 목표 프레임에 도달
- 두 유닛이 동시에 목표에 있어야 함

## 실패 조건
- 격자 밖 이동 시도는 차단됨
- 벽에 충돌하는 이동은 차단됨
- 이동 제한이 있는 스테이지에서 제한 초과 시 실패
  - 상단에 남은 이동 수가 표시됨

## 조작 방법
### 데스크톱(키보드)
- 위: 방향키 ↑
- 아래: 방향키 ↓
- 왼쪽: 방향키 ←
- 오른쪽: 방향키 →

### 모바일(터치)
- 위로 스와이프: 위 이동
- 아래로 스와이프: 아래 이동
- 왼쪽 스와이프: 왼쪽 이동
- 오른쪽 스와이프: 오른쪽 이동
- 스테이지 클리어 후 위로 스와이프 또는 탭: 다음 스테이지
- 힌트 보기: `H` 키 또는 상단 상태 텍스트 롱프레스
- 힌트는 여러 번 호출하면 순환 표시됨

## 진행 방식
- 스테이지는 `levels.json` 순서대로 로드됩니다(난이도 구간 내에서 랜덤).
- 캠페인은 총 118 스테이지이며, 마지막 클리어 후 처음으로 루프됩니다.
- JSON 로드 실패 시 랜덤 스테이지로 진행됩니다.
- 스테이지 1에서는 튜토리얼 힌트가 로그에 표시됩니다.
- 상단에 남은 이동 수 바가 표시됩니다.

## 특수 타일(있는 경우)
- 벽: 이동 불가
- 슬립 타일: 같은 방향으로 1칸 추가 이동
- 포털: 페어 포털로 즉시 이동
- 금지 타일: 녹색 유닛만 통과 불가
- 역전 타일(분홍 다이아): 다음 1턴 동안 같은 방향 이동

## 팁
- 녹색 유닛과 빨간 유닛을 동시에 계획하세요.
- 가장자리로 빨간 유닛 위치를 조절하세요.

## 저작권
- 모든 권리는 Tangle-Studio에 있습니다.

---

## Overview
Tangle-Ops is a grid-based puzzle game. Move the green unit while the red
entangled unit moves in the opposite direction. Clear a stage by placing both
units on their target frames at the same time.

## Win Condition
- Green unit reaches the green target frame.
- Red unit reaches the red target frame.
- Both must be on their targets simultaneously.

## Failure Conditions
- If a move would go out of bounds, the move is blocked.
- If a move would hit a wall, the move is blocked.
- In stages with a move limit, exceeding the limit fails the stage.
  - Remaining moves are shown at the top.

## Controls
### Desktop (Keyboard)
- Move Up: Arrow Up
- Move Down: Arrow Down
- Move Left: Arrow Left
- Move Right: Arrow Right

### Mobile (Touch)
- Swipe Up: move up
- Swipe Down: move down
- Swipe Left: move left
- Swipe Right: move right
- After clearing a stage, swipe up or tap to go to the next stage
- Show hint: press `H` or long-press the top status text
- Repeat hint triggers to cycle through multiple hints

## Stage Progression
- Stages load from `levels.json` with random order inside each difficulty tier.
- Campaign has 118 stages; after the final stage, the game loops back to the first.
- If JSON loading fails, the game uses random stages.
- Stage 1 shows tutorial hints in the log.
- A move limit bar appears at the top when active.

## Special Tiles (if present)
- Wall: blocks movement.
- Slip tile: forces one extra move in the same direction.
- Portal: teleports to its paired portal.
- Forbidden tile: blocks the green unit only.
- Inversion tile (pink diamond): the next move makes both units move in the same direction.

## Tips
- Plan both units together, not just the green one.
- Use the edges to control the red unit’s position.

## Copyright
- © Tangle-Studio. All rights reserved.

