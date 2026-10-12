# 배너 기준

배너는 [WhiteKiwi PIP](https://github.com/WhiteKiwi/kiwi-design-system)의 저장소 디자인 규칙을 따릅니다.
적용한 기준 커밋은 `54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3`입니다.

- [Repository surfaces](https://github.com/WhiteKiwi/kiwi-design-system/blob/54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3/docs/repository-surfaces.md)
- [Semantic tokens](https://github.com/WhiteKiwi/kiwi-design-system/blob/54cefe89bf08e1bd77aa4ce2b7f8d6e2386001a3/packages/tokens/src/theme.css)

| 역할 | Light | Dark |
| :--- | :--- | :--- |
| Canvas | `#F4F5EF` | `#0E100E` |
| Text | `#11140F` | `#F1F4EB` |
| Text muted | `#62685E` | `#A5AB9F` |
| Kiwi headline | `#3C6000` | `#C6FF4A` |

`KEEP THE GOOD.`라는 짧은 제목 하나를 넓은 여백에 배치합니다.
초록색은 `GOOD.`에만 사용합니다. 본문과 이동 링크는 GitHub의 기본 Markdown을 사용합니다.

Desktop은 `banner-light.svg`와 `banner-dark.svg`를 사용합니다.
600px 이하 viewport에서는 `banner-mobile-light.svg`와 `banner-mobile-dark.svg`로 구성을 바꿉니다.
모든 배너는 자체 포함 SVG이며 외부 폰트, 스크립트, 애니메이션을 사용하지 않습니다.

색상을 바꿀 때는 원본 토큰과 foreground/background 대비를 확인하고,
light·dark 및 320px·390px에서 실제 렌더링을 점검합니다.
