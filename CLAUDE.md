# 우리팀 카페 — 팀 규칙

모든 팀원(과 Claude)은 아래 규칙을 항상 지킨다.

1. **HTML과 CSS만 사용한다.** JavaScript 등 다른 언어는 쓰지 않는다.
2. **디자인은 `style.css`를 연결해서 쓴다.** `<link rel="stylesheet" href="style.css">`를 넣고, `style.css`는 수정하지 않는다.
3. **메뉴는 `.menu-card` 모양으로 만든다.**
4. **메뉴 페이지 맨 아래에는 "처음으로" 링크를 넣는다.** (`index.html`로 연결)
5. **자기 담당 파일 외의 파일은 수정하지 않는다.**
6. **GitHub에 올릴 때는 작업 브랜치에만 올리고 `main`에는 병합하지 않는다.** `main`으로 합치는 일은 GitHub에서 Pull Request(Compare & pull request → Create pull request → Merge pull request)로 한다. "커밋하고 GitHub에 올려줘"라고 해도 마찬가지이며, 개인 설정의 "기본 브랜치까지 병합" 규칙보다 이 규칙을 먼저 따른다.

## 파일 구성

| 파일 | 내용 |
|---|---|
| `index.html` | 첫 화면 (카페 이름, 환영 문구, 메뉴 버튼 3개) |
| `style.css` | 모든 페이지 공통 디자인 |
| `drinks.html` | 음료 메뉴 |
| `desserts.html` | 디저트 메뉴 |
| `today.html` | 오늘의 추천 |

## 메뉴 페이지 예시

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>음료 | 우리팀 카페</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h2>음료</h2>

  <div class="menu-list">
    <div class="menu-card">
      <h3>아메리카노</h3>
      <p>깔끔하고 진한 기본 커피</p>
      <p class="price">4,000원</p>
    </div>
  </div>

  <a class="home-link" href="index.html">처음으로</a>
</body>
</html>
```
