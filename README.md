# 🏕️ delicious_dish_for_camping

캠핑 요리 전문가 봇 — Claude Code 스킬.

캠핑 상황(인원·장비·계절·난이도)에 맞춰 **메뉴 → 재료 → 조리법** 순서로 요리를 안내합니다.

## 구성

```
delicious_dish_for_camping/
├── SKILL.md            # 스킬 정의 (봇 페르소나 + 응답 흐름)
├── recipes/
│   └── recipes.md      # 기본 레시피 데이터
└── README.md
```

## 설치 (Claude Code에서 스킬로 사용하기)

스킬 디렉토리에 심볼릭 링크하거나 복사합니다.

```bash
# 심볼릭 링크 (레포 수정이 바로 반영됨)
ln -s "$(pwd)" ~/.claude/skills/camping-chef

# 또는 복사
cp -r "$(pwd)" ~/.claude/skills/camping-chef
```

이후 Claude Code에서 "캠핑 메뉴 추천해줘" 같은 요청을 하면 자동으로 발동합니다.

## 사용 예시

```
나: 4명이서 화로대 가지고 캠핑 가는데 메뉴 추천해줘

봇:
🏕️ 추천 메뉴
- 불멍 삼겹살: 화로대 입문, 설거지 적음
- 차돌된장: 밥도둑, 쌈 곁들임
...
🛒 재료 (4인 기준)
...
🔥 조리법
1. ...
💡 캠핑 꿀팁
...
```

## 레시피 추가하기

`recipes/recipes.md`에 같은 형식(메뉴 → 재료 → 조리법)으로 추가하면 봇이 참고합니다.
