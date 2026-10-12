# AGENTS.md

`WhiteKiwi/awesome`은 WhiteKiwi가 마음에 든 글, 영상, 도구와 발견을 모으는 개인 컬렉션입니다.
이 파일을 작성·분류·관리의 기준으로 사용합니다.

## 파일 역할

- `README.md`: 방문자가 자료를 고르는 첫 화면입니다. 배너, 짧은 소개, 카테고리 이동, 최근 자료와 추천 링크를 배치합니다.
- `collection/*.md`: 전체 목록의 원본입니다. 자료의 원제목, 원문 링크, 설명, 태그와 저장 날짜를 기록합니다.
- `AGENTS.md`: 작성 형식, 관리 절차, 디자인 기준과 검증 방법을 둡니다.
- `.github/ISSUE_TEMPLATE/save-link.yml`: 링크를 빠르게 남기는 Inbox 양식입니다. 자료 형식은 자유 입력을 유지합니다.
- `assets/banner-light.svg`, `assets/banner-dark.svg`: README의 라이트·다크 배너입니다.

## 링크 기록

```markdown
- [원래 제목](원문-URL) — 자료의 내용이나 좋았던 이유 한 문장. `태그` · YYYY-MM-DD
```

- 사용자가 고른 자료를 모읍니다. 새 자료를 임의로 추가하거나 취향을 대신 결정하지 않습니다.
- 제목과 내용을 원문에서 확인합니다. 사용자가 이유를 말하지 않았다면 내용 중심으로 설명하고, 감상이나 시청·독서 상태를 추측하지 않습니다.
- 원문 전체나 긴 인용을 옮기지 않습니다. 목록과 직접 작성한 메모는 CC0이며, 링크된 콘텐츠의 권리는 원저작자에게 있습니다.
- 태그와 날짜는 선택입니다. 날짜는 발행일이 아닌 저장한 날이며, 사용자의 현지 날짜를 사용합니다.
- 각 카테고리에서는 최근에 담은 항목을 위에 둡니다. 날짜가 같으면 기존 순서를 유지합니다.
- 같은 자료가 이미 있는지 확인하고 가장 잘 맞는 카테고리 하나에 기록합니다.
- 불필요한 추적 매개변수는 제거합니다. 영상 ID, 타임스탬프 등 내용을 지정하는 값은 유지합니다.

## 카테고리 관리

- 첫 자료를 담을 때 새 카테고리를 만듭니다. 빈 카테고리나 빈 상태 안내를 미리 만들지 않습니다.
- 새 파일은 `collection/{kebab-slug}.md`로 만들고 제목, README로 돌아가는 링크, 짧은 소개, `모아둔 것들`과 첫 항목을 함께 추가합니다.
- 새 카테고리를 README의 이동 링크와 자료 섹션에도 추가합니다. 실제 자료가 있는 카테고리만 표시합니다.
- 항목이 많아져 탐색이 어려워지면 해당 카테고리 안에 주제별 제목을 추가합니다.

## README 편집

- 소개와 실제 자료를 먼저 보여줍니다. 작성 예시, 파일 구조, 운영 절차와 검증 설명은 이 파일에 둡니다.
- `collection/*.md`를 기준으로 각 카테고리의 최근 자료를 최대 3개씩 소개합니다. 목록을 바꾸면 README 미리보기도 같은 작업에서 갱신합니다.
- 각 자료는 원문으로 연결되는 제목, 짧은 설명, 출처와 주제를 표시합니다. 영상 길이는 확인한 경우에만 적습니다.
- README의 표시 제목은 뜻을 유지하며 짧게 다듬을 수 있습니다. 원제목은 컬렉션에 그대로 보존합니다.
- 새 카테고리를 만들면 이동 링크, 섹션 제목과 전체 목록 링크를 함께 추가합니다.
- 추천 링크는 짧게 안내합니다. AI 작업 지침과 내부 관리 설명을 방문자의 읽기 흐름에 넣지 않습니다.

## Inbox 정리

1. 이슈의 원문 링크와 제목을 확인하고 기존 목록과 중복을 확인합니다.
2. 적절한 카테고리에 자료를 기록하고 README 미리보기를 갱신합니다.
3. 저장소에 반영된 항목을 확인한 뒤 해당 Inbox 이슈를 닫습니다.

Inbox 이슈나 Pull Request로 받은 추천의 최종 선택은 WhiteKiwi의 취향을 따릅니다.

## 디자인 기준

[WhiteKiwi PIP](https://github.com/WhiteKiwi/kiwi-design-system)를 따릅니다.
배너 기준 커밋은 `54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3`입니다.

- [Repository surfaces](https://github.com/WhiteKiwi/kiwi-design-system/blob/54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3/docs/repository-surfaces.md)
- [Semantic tokens](https://github.com/WhiteKiwi/kiwi-design-system/blob/54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3/packages/tokens/src/theme.css)

| 역할 | Light | Dark |
| :--- | :--- | :--- |
| Canvas | `#F4F5EF` | `#0E100E` |
| Text | `#11140F` | `#F1F4EB` |
| Text muted | `#62685E` | `#A5AB9F` |
| Kiwi headline | `#3C6000` | `#C6FF4A` |

- 넓은 여백과 정렬을 먼저 사용합니다. 배너는 짧은 제목 하나를 맡고, 초록색 강조는 `GOOD.`에 집중합니다.
- 본문, 제목과 이동 링크는 GitHub의 기본 Markdown을 사용합니다. 자료 목록은 좁은 화면에서도 자연스럽게 줄바꿈하도록 배치합니다.
- 배너는 `viewBox`, title/description과 유용한 alt text가 있는 자체 포함 SVG로 유지합니다. 외부 폰트, 스크립트와 애니메이션을 추가하지 않습니다.
- `<picture>`는 라이트·다크 소스와 라이트 fallback을 사용합니다. GitHub가 media 조건을 다시 작성하므로 테마 조건에 화면 폭 조건을 섞지 않습니다.
- 색상을 바꾸면 기준 토큰과 실제 foreground/background 대비를 다시 확인합니다. 일반 텍스트는 4.5:1, 큰 텍스트는 3:1 이상을 기준으로 합니다.

구성 참고:

- [sindresorhus/awesome](https://github.com/sindresorhus/awesome): 카테고리 목차와 일관된 링크 설명.
- [EanNewton/Awesome-Reading-List](https://github.com/EanNewton/Awesome-Reading-List): 최근 자료와 짧은 설명·메타데이터.
- [bartolomej/bookmarks](https://github.com/bartolomej/bookmarks): 개인 컬렉션의 소개와 카테고리 탐색.

## 검증과 Git

- 상대 링크, 카테고리 이동 링크와 원문 URL이 올바른지 확인합니다.
- README의 자료가 컬렉션 원본과 맞는지, 빈 카테고리가 생기지 않았는지 확인합니다.
- Markdown을 바꾸면 GitHub 렌더링과 320px·390px·데스크톱에서 제목, 한국어 줄바꿈과 가로 넘침을 확인합니다. 배너를 바꾸면 라이트·다크도 함께 확인합니다.
- 이슈 양식을 바꾸면 YAML 문법과 필수 입력 필드를 확인합니다.
- `git diff --check`로 형식을 확인하고 변경 범위와 검증 결과를 짧게 보고합니다.
- 커밋 제목은 `{type}: {message}` 형식을 사용합니다. `type`은 소문자로, `message`는 구체적인 동작으로 적습니다.
