# AI창의융합코딩연구반 개인 포트폴리오 실습 가이드

오늘 만든 포트폴리오 사이트는 아주 작은 전시 공간입니다.  
`index.html`은 전시장 구조, `style.css`는 전시장 꾸미기, `script.js`는 버튼과 기록 기능, `club-logo.png`는 동아리 간판입니다.

완성 파일은 다음 5개입니다.

- `index.html`
- `style.css`
- `script.js`
- `club-logo.png`
- `practice-guide.md`

## 1. 오늘 실습에서 바꾸는 곳

오늘의 목표는 "남이 만든 예쁜 페이지를 보는 것"이 아니라 "내가 수행한 활동이 드러나는 개인 포트폴리오로 바꾸는 것"입니다.

처음 웹사이트를 게시하는 학생이라면 코드를 전부 이해하려고 하면 어렵게 느껴질 수 있습니다.  
먼저 아래 순서대로 접근하세요.

1. `index.html`에서 화면에 보이는 글을 내 정보로 바꿉니다.
2. `script.js`에서 동아리 활동, 프로젝트 카드, 처음 보이는 기록 예시를 내 활동으로 바꿉니다.
3. `style.css`에서 색상과 분위기를 조금만 바꿔 봅니다.
4. 브라우저에서 새로고침해서 화면이 어떻게 달라졌는지 확인합니다.
5. 마음에 들면 CodePen과 GitHub Pages에 올려 확인합니다.

코드 안의 `수정:` 주석은 선생님이 붙여 둔 작은 포스트잇입니다.  
하지만 주석만 찾고 끝내면 안 됩니다. 아래 예시처럼 "원래 문장"을 "내 문장"으로 바꾸는 연습을 해야 진짜 개인 포트폴리오가 됩니다.

### 수정할 때 지켜야 할 쉬운 규칙

- 따옴표 `" "` 안의 글을 바꿀 때는 따옴표를 지우지 않습니다.
- `<h1>내용</h1>`처럼 태그 사이의 글을 바꿀 때는 `<h1>`과 `</h1>`은 그대로 둡니다.
- `[`와 `]`, `{`와 `}`, `,`는 JavaScript에서 중요한 기호입니다. 글만 바꾸고 기호는 조심해서 유지합니다.
- 한 번에 너무 많이 바꾸지 말고, 2~3곳을 바꾼 뒤 저장하고 새로고침합니다.

### `index.html`에서 바꾸는 것

`index.html`은 화면에 보이는 글과 순서를 담당합니다.

쉽게 말하면 자기소개서의 본문입니다.  
내 이름, 큰 제목, 자기소개, 연락처처럼 "사람이 읽는 문장"은 대부분 이 파일에 있습니다.

바꾸기 좋은 곳은 다음과 같습니다.

- 브라우저 제목: `<title>AI창의융합코딩연구반 포트폴리오</title>`
- 왼쪽 위 로고 글자: `<span class="logo-mark">AI</span>`
- 큰 제목: `<h1 id="hero-title">...</h1>`
- 자기소개 문장
- 이름, 학년, 관심 분야
- 관심 키워드 목록
- 배운 점 3개
- 이메일, GitHub 주소

예를 들어 이름을 바꾸고 싶다면 아래처럼 고칩니다.  
이때 `<h2>`와 `</h2>`는 지우지 말고, 가운데 글자만 바꿉니다.

```html
<h2>홍길동</h2>
```

를

```html
<h2>김민지</h2>
```

### `index.html`에서 바로 바꿔 볼 수 있는 예시

아래 예시는 그대로 따라 해도 되고, 자기 상황에 맞게 더 바꿔도 됩니다.

1. 브라우저 탭 제목 바꾸기

```html
<title>AI창의융합코딩연구반 포트폴리오</title>
```

```html
<title>김민지의 AI 포트폴리오</title>
```

2. 왼쪽 위 작은 로고 글자 바꾸기

```html
<span class="logo-mark">AI</span>
```

```html
<span class="logo-mark">MJ</span>
```

3. 첫 화면 큰 제목 바꾸기

```html
<h1 id="hero-title">코딩으로 생각을 만들고, AI로 가능성을 넓힙니다.</h1>
```

```html
<h1 id="hero-title">AI와 코딩으로 나의 아이디어를 직접 만들어 봅니다.</h1>
```

4. 자기소개 문장 바꾸기

```html
안녕하세요. 저는 문제를 관찰하고, 작은 아이디어를 코드로 구현하는 과정을 좋아하는 학생입니다.
```

```html
안녕하세요. 저는 생활 속 불편함을 찾아보고, AI와 웹 기술로 해결 방법을 만들어 보는 학생입니다.
```

5. 이름과 학년 바꾸기

```html
<h2>홍길동</h2>
<p>영신여고 1학년 · AI와 웹 개발에 관심 있는 학생</p>
```

```html
<h2>김민지</h2>
<p>영신여고 2학년 · 데이터 분석과 AI 활용에 관심 있는 학생</p>
```

6. 관심 분야 바꾸기

```html
<dd>AI, 웹, 데이터</dd>
```

```html
<dd>AI 챗봇, 앱 디자인, 발표 자료 만들기</dd>
```

7. 관심 키워드 목록 바꾸기

```html
<li>웹 페이지 만들기</li>
<li>AI 프롬프트 실험</li>
```

```html
<li>학교생활 도우미 챗봇</li>
<li>학습 기록 자동 정리</li>
```

8. 동아리 로고 설명 바꾸기

```html
실습 결과물과 포트폴리오에 함께 사용할 수 있는 AI창의융합코딩연구반 대표 이미지입니다.
```

```html
우리 동아리의 활동 방향을 보여 주는 로고입니다. AI와 코딩을 활용한 창의적인 결과물을 기록합니다.
```

9. 배운 점 제목 바꾸기

```html
<h3>작게 시작하기</h3>
```

```html
<h3>오류를 기록하며 해결하기</h3>
```

10. 이메일 주소 바꾸기

```html
<a href="mailto:student@example.com">student@example.com</a>
```

```html
<a href="mailto:minji@example.com">minji@example.com</a>
```

11. GitHub 주소 바꾸기

```html
<a href="https://github.com/" target="_blank" rel="noreferrer">GitHub</a>
```

```html
<a href="https://github.com/my-id" target="_blank" rel="noreferrer">GitHub</a>
```

12. 맨 아래 문구 바꾸기

```html
<p>2026 AI창의융합코딩연구반 · 나의 첫 개인 포트폴리오</p>
```

```html
<p>2026 AI창의융합코딩연구반 · 김민지의 성장 기록</p>
```

### `script.js`에서 바꾸는 것

`script.js`는 프로젝트 카드, 동아리 활동, 포트폴리오 기록 기능을 담당합니다.  
버튼을 누르면 화면이 바뀌게 해 주는 리모컨 역할입니다.  
처음에는 복잡해 보이지만, 대부분은 "제목", "설명", "태그" 같은 글을 바꾸는 일입니다.

바꾸기 좋은 곳:

- `activityData`: 동아리 활동 기록
- `projectData`: 프로젝트 카드 내용
- `starterNoteData`: 처음 화면에 보이는 예시 기록

프로젝트를 바꾸고 싶다면 `projectData` 안의 제목과 설명을 고칩니다.

```js
{
  title: "AI 아이디어 노트",
  description: "AI에게 질문하고 받은 답변을 비교하며 좋은 프롬프트의 조건을 정리했습니다.",
  category: "ai",
  icon: "AI",
  tags: ["AI", "프롬프트", "기록"],
}
```

`category`는 필터 버튼과 연결됩니다.

- `web`: 웹 프로젝트
- `ai`: AI 활용 프로젝트
- `data`: 데이터 프로젝트

### `script.js`에서 바로 바꿔 볼 수 있는 예시

13. 동아리 활동 월과 제목 바꾸기

```js
{
  date: "3월",
  title: "HTML 구조 익히기",
  description: "제목, 문단, 링크, 목록 태그를 사용해 첫 웹 페이지를 만들었습니다.",
}
```

```js
{
  date: "3월",
  title: "나의 관심 분야 정리하기",
  description: "AI와 코딩으로 해결해 보고 싶은 문제를 생각하고 포트폴리오 주제를 정했습니다.",
}
```

14. 프로젝트 카드 제목 바꾸기

```js
title: "나를 소개하는 웹 페이지",
```

```js
title: "학교생활 도우미 웹 페이지",
```

15. 프로젝트 설명 바꾸기

```js
description: "HTML과 CSS를 사용해 자기소개, 관심 분야, 목표를 정리한 첫 페이지입니다.",
```

```js
description: "학교생활에서 자주 확인하는 일정과 준비물을 한 화면에 정리한 웹 페이지입니다.",
```

16. 프로젝트 분류 바꾸기

```js
category: "web",
```

```js
category: "ai",
```

분류를 `ai`로 바꾸면 `AI` 필터 버튼을 눌렀을 때 보입니다.

17. 프로젝트 아이콘 글자 바꾸기

```js
icon: "WEB",
```

```js
icon: "APP",
```

18. 프로젝트 태그 바꾸기

```js
tags: ["HTML", "CSS", "기초"],
```

```js
tags: ["기획", "AI", "발표"],
```

19. 처음 보이는 예시 기록 바꾸기

```js
title: "첫 포트폴리오 구조 만들기",
content: "HTML 섹션을 나누고 자기소개, 활동, 프로젝트 영역을 만들었습니다.",
```

```js
title: "프로젝트 아이디어 정리",
content: "내가 해결하고 싶은 문제를 적고, 어떤 기능이 필요할지 간단히 목록으로 만들었습니다.",
```

20. 기록 저장 이름은 그대로 두기

```js
const notesStorageKey = "ysPortfolioNotes";
```

이 부분은 브라우저가 기록을 저장할 때 쓰는 이름입니다.  
수업 중에는 바꾸지 않는 것이 좋습니다. 이미 저장한 기록과 연결되어 있기 때문입니다.

### `style.css`에서 바꾸는 것

`style.css`는 색, 크기, 여백, 카드 모양을 담당합니다.  
옷을 갈아입히는 파일이라고 생각하면 쉽습니다.

처음에는 전체 구조를 바꾸기보다 맨 위의 색상 변수만 바꿔 보는 것을 추천합니다.

```css
:root {
  --color-bg: #f7f8f3;
  --color-primary: #0f766e;
  --color-warm: #f6c453;
}
```

색상 코드는 물감 번호처럼 생각하면 됩니다. `#0f766e`는 초록빛, `#2563eb`는 파란빛입니다.

### `style.css`에서 바로 바꿔 볼 수 있는 예시

21. 대표 색을 파란색으로 바꾸기

```css
--color-primary: #0f766e;
```

```css
--color-primary: #2563eb;
```

22. 따뜻한 포인트 색을 분홍색으로 바꾸기

```css
--color-warm: #f6c453;
```

```css
--color-warm: #f9a8d4;
```

23. 배경을 조금 더 밝게 바꾸기

```css
--color-bg: #f7f8f3;
```

```css
--color-bg: #fbfbff;
```

24. 카드 둥근 정도 바꾸기

```css
--radius: 8px;
```

```css
--radius: 4px;
```

숫자가 작을수록 더 각진 카드가 되고, 숫자가 클수록 더 둥근 카드가 됩니다.

25. 큰 제목 크기를 조금 줄이기

```css
h1 {
  font-size: 4.8rem;
}
```

```css
h1 {
  font-size: 4.2rem;
}
```

제목이 너무 크게 느껴질 때만 바꿉니다. 휴대폰 화면 크기는 아래쪽 `@media` 안에서 따로 조절됩니다.

### 포트폴리오 기록 기능

사이트 중간에 `포트폴리오 기록` 섹션이 있습니다.  
여기에는 오늘 한 활동을 간단히 적을 수 있습니다.

예시:

- 기록 제목: `첫 웹 페이지 완성`
- 활동 종류: `실습`
- 기록 내용: `HTML로 자기소개 영역을 만들고 CSS로 카드 모양을 꾸몄다.`

`기록 추가` 버튼을 누르면 아래 목록에 바로 나타납니다.

중요한 점:

- 이 기록은 복잡한 데이터베이스를 쓰지 않습니다.
- 현재 브라우저 안에 저장됩니다.
- 같은 컴퓨터, 같은 브라우저에서는 새로고침해도 남아 있습니다.
- 브라우저 기록을 지우거나 다른 컴퓨터로 가면 사라질 수 있습니다.

비유하면 책상 위 개인 메모지입니다. 친구 책상이나 학교 서버에 자동으로 붙는 메모는 아닙니다.

### 기록 기능으로 남기기 좋은 메모 예시

포트폴리오는 완성작만 보여 주는 곳이 아닙니다.  
"무엇을 시도했고, 무엇을 배웠는지"를 적어 두면 나중에 발표나 생활기록부 세특을 정리할 때도 도움이 됩니다.

예시로는 이런 문장을 넣을 수 있습니다.

1. `HTML로 자기소개 영역을 만들고, 제목과 문단 태그의 차이를 알게 되었다.`
2. `CSS 색상 변수를 바꾸어 사이트 분위기가 어떻게 달라지는지 확인했다.`
3. `프로젝트 카드 내용을 내 활동에 맞게 수정했다.`
4. `AI에게 질문할 때 조건을 자세히 적으면 답변이 더 정확해진다는 것을 배웠다.`
5. `JavaScript 배열에 새 프로젝트를 추가해 화면에 카드가 생기는 것을 확인했다.`
6. `GitHub Pages에 파일을 올리고 인터넷 주소로 접속해 보았다.`
7. `로고 이미지가 보이지 않는 문제를 파일 이름과 위치를 확인해 해결했다.`
8. `모바일 화면에서 글자가 겹치지 않는지 확인했다.`
9. `오류가 났을 때 바로 지우지 않고 어떤 메시지가 나오는지 먼저 읽어 보았다.`
10. `오늘 만든 결과물을 친구에게 보여 주고 어떤 부분을 더 고치면 좋을지 의견을 들었다.`

## 2. CodePen에서 화면 확인하기

CodePen은 코드를 바로 붙여 넣고 결과를 보는 실습장입니다.  
종이에 설계도를 그리자마자 옆에서 모형이 만들어지는 곳이라고 생각하면 됩니다.

### CodePen에 넣는 방법

1. CodePen에서 새 Pen을 만듭니다.
2. HTML 패널에는 `index.html`의 `<body>` 안쪽 내용을 넣습니다.
   - `<header class="site-header">`부터 `<footer class="site-footer">...</footer>`까지 복사하면 됩니다.
   - `<html>`, `<head>`, `<body>`, `<link rel="stylesheet">`, `<script src="script.js">` 줄은 CodePen에서는 보통 넣지 않아도 됩니다.
3. CSS 패널에는 `style.css` 전체를 붙여 넣습니다.
4. JS 패널에는 `script.js` 전체를 붙여 넣습니다.
5. 결과 화면에서 글, 카드, 버튼, 기록 추가 기능이 작동하는지 확인합니다.

### CodePen에서 동아리 로고 이미지는 어떻게 하나요?

이 사이트는 `club-logo.png` 파일을 사용합니다.  
GitHub Pages에서는 같은 폴더에 `club-logo.png`를 올리면 바로 보입니다.

CodePen에서는 이미지 파일을 직접 같이 올리는 방식이 계정 상태에 따라 다를 수 있습니다. 그래서 실습 때는 아래 중 하나를 선택하면 됩니다.

- 쉬운 방법: CodePen에서는 로고가 안 보여도 글과 레이아웃 실습을 먼저 합니다.
- 이미지 주소 사용: 나중에 GitHub Pages에 올린 뒤 이미지 주소를 복사해서 `src="club-logo.png"` 대신 넣습니다.
- 업로드 기능 사용: CodePen에서 이미지 업로드가 가능한 계정이면 업로드한 이미지 주소를 `src`에 넣습니다.

예시:

```html
<img class="club-logo-image" src="club-logo.png" alt="2026 AI창의융합 코딩연구반 로고" />
```

를

```html
<img class="club-logo-image" src="이미지주소" alt="2026 AI창의융합 코딩연구반 로고" />
```

처럼 바꿉니다.

### CodePen에서 꼭 확인할 것

- 큰 제목이 내 문장으로 바뀌었는가?
- 이름과 자기소개가 내 정보로 바뀌었는가?
- 프로젝트 카드가 내가 한 활동으로 바뀌었는가?
- `전체`, `웹`, `AI`, `데이터` 버튼이 작동하는가?
- `포트폴리오 기록`에 메모를 넣으면 바로 보이는가?
- 휴대폰 크기로 줄여도 글자가 겹치지 않는가?

## 3. GitHub Pages로 게시하기

GitHub Pages는 내 파일을 인터넷에 올려서 주소로 볼 수 있게 해 주는 기능입니다.  
학교 게시판에 작품을 붙이는 일과 비슷합니다.

### GitHub 웹사이트에서 올리는 쉬운 방법

1. GitHub에 로그인합니다.
2. 오른쪽 위 `+` 버튼을 누르고 `New repository`를 선택합니다.
3. 저장소 이름을 정합니다.
   - 예: `my-ai-portfolio`
4. 공개 범위는 수업용이면 `Public`으로 둡니다.
5. `Create repository`를 누릅니다.
6. 저장소 화면에서 `uploading an existing file` 또는 `Add file` > `Upload files`를 선택합니다.
7. 아래 파일을 모두 끌어다 놓습니다.
   - `index.html`
   - `style.css`
   - `script.js`
   - `club-logo.png`
   - `practice-guide.md`
8. 아래쪽 `Commit changes`를 누릅니다.
   - 화면에 `Propose changes`라고 보이면 그 버튼을 눌러도 됩니다.

여기서 `Commit changes`는 사진을 찍어 저장하는 일과 비슷합니다.  
파일 상태를 한 장의 사진처럼 남기는 것입니다.

### GitHub Pages 켜기

1. 저장소에서 `Settings`로 들어갑니다.
2. 왼쪽 메뉴에서 `Pages`를 찾습니다.
3. `Build and deployment`에서 `Source`를 `Deploy from a branch`로 선택합니다.
4. `Branch`를 `main`, 폴더를 `/(root)`로 선택합니다.
5. `Save`를 누릅니다.
6. 잠시 기다리면 Pages 주소가 생깁니다.

주소 예시:

```text
https://아이디.github.io/my-ai-portfolio/
```

처음에는 1분에서 몇 분 정도 기다려야 할 수 있습니다.  
바로 안 보이면 새로고침하거나 조금 있다가 다시 확인합니다.

### GitHub Pages에서 안 보일 때 확인할 것

- 파일 이름이 정확히 `index.html`인가?
- `index.html`이 폴더 안쪽이 아니라 저장소 첫 화면에 있는가?
- `style.css`, `script.js`, `club-logo.png`가 `index.html`과 같은 위치에 있는가?
- Pages 설정에서 branch가 `main`, folder가 `/(root)`인가?
- 주소 끝에 저장소 이름이 들어갔는가?

## 4. 더 깊게 배우기: 내 컴퓨터에서 Git과 GitHub로 올리기

여기부터는 조금 더 진짜 개발자 방식입니다.  
Git은 내 파일의 변화 과정을 기록하는 도구이고, GitHub는 그 기록을 인터넷에 보관하는 공간입니다.

주의할 점이 있습니다.  
GitHub 웹사이트에서 파일을 올리는 방법은 맥북과 윈도우가 거의 비슷하지만, Git 명령어를 입력하는 부분은 운영 체제의 영향을 받습니다.  
특히 "터미널을 어디서 여는지", "폴더 주소를 어떻게 쓰는지", "파일 목록을 확인하는 명령어가 무엇인지"가 다릅니다.

쉬운 비유:

- 작업 폴더: 내 책상
- `git add`: 제출할 종이를 봉투에 넣기
- `git commit`: 봉투에 제목을 쓰고 사진 찍기
- `git push`: GitHub라는 온라인 보관함에 보내기

### 먼저 내 컴퓨터 종류를 확인하세요

자신의 컴퓨터에 맞는 설명을 따라가면 됩니다.

- 맥북 사용자: 아래 `맥북에서 Git 사용하기`를 봅니다.
- 윈도우 사용자: 아래 `윈도우에서 Git 사용하기`를 봅니다.
- 학교 컴퓨터라 설치 권한이 없으면: GitHub 웹사이트에서 파일 업로드하는 쉬운 방법을 사용합니다.

### 명령어를 배우기 전에 끝내야 할 사전 세팅

초보자가 가장 많이 막히는 부분은 `git add`, `git commit` 같은 명령어 자체보다 그 전에 필요한 준비입니다.  
아래 준비가 되어 있지 않으면 마지막 `git push`에서 파일이 GitHub 저장소로 올라가지 않을 수 있습니다.

#### 공통 준비물

맥북과 윈도우 모두 아래 준비가 필요합니다.

- GitHub 계정이 있어야 합니다.
- GitHub 계정 이메일 인증이 끝나 있어야 합니다.
- 인터넷에 연결되어 있어야 합니다.
- 내 포트폴리오 파일이 한 폴더 안에 모여 있어야 합니다.
- 그 폴더 안에 `index.html`, `style.css`, `script.js`, `club-logo.png`, `practice-guide.md`가 있어야 합니다.
- GitHub에 비어 있는 새 저장소를 만들어 두어야 합니다.
- 저장소 주소는 HTTPS 주소를 사용합니다.

저장소 주소는 이런 모양이면 좋습니다.

```text
https://github.com/내아이디/my-ai-portfolio.git
```

수업에서는 SSH 주소보다 HTTPS 주소를 추천합니다.  
SSH는 키를 따로 만들고 GitHub에 등록해야 해서 처음 게시하는 학생에게는 단계가 더 많습니다.

#### GitHub 계정 준비

GitHub에 로그인한 뒤 아래를 확인합니다.

1. 이메일 인증이 끝났는지 확인합니다.
2. 저장소를 만들 수 있는지 확인합니다.
3. 새 저장소 이름을 정합니다. 예: `my-ai-portfolio`
4. 저장소를 만들 때 `Public`으로 둡니다.
5. 처음에는 README, `.gitignore`, license를 자동으로 만들지 않는 것이 쉽습니다.

이미 README를 만들어 버렸다면 큰 문제는 아니지만, 첫 `git push`에서 충돌이 날 수 있습니다.  
처음 배우는 수업에서는 빈 저장소를 만드는 것이 가장 안전합니다.

#### Git 인증 준비

GitHub는 예전처럼 터미널에 GitHub 비밀번호를 직접 입력해서 `push`하는 방식을 권장하지 않습니다.  
수업에서는 아래 두 방법 중 하나를 사용하면 됩니다.

- 추천: Git Credential Manager가 띄우는 브라우저 로그인 창에서 로그인하기
- 대안: Personal Access Token을 만들어 비밀번호 대신 사용하기

처음 학생에게는 Git Credential Manager 방식이 더 쉽습니다.  
`git push`를 입력했을 때 브라우저 로그인 창이 뜨면 GitHub에 로그인하고 허용하면 됩니다.

Personal Access Token은 비밀번호처럼 조심히 다루어야 하므로, 수업에서는 선생님 안내 없이 만들지 않는 것을 권장합니다.

### 맥북에서 Git 사용하기

맥북에서는 `터미널` 앱을 사용합니다.  
화면 위쪽 검색 기능인 Spotlight에서 `터미널` 또는 `Terminal`을 검색해 열 수 있습니다.

#### Mac 0단계: 설치와 인증 환경 준비

맥북에서는 Git이 이미 준비되어 있는 경우가 많지만, 처음 실행할 때 Xcode Command Line Tools 설치 창이 뜰 수 있습니다.  
이 창은 이상한 오류가 아니라 "Git을 실행하는 데 필요한 도구를 설치하라"는 안내입니다.

맥북 사용자는 수업 전에 아래를 확인합니다.

1. `터미널` 앱을 열 수 있는지 확인합니다.
2. `git --version`을 실행해 Git이 있는지 확인합니다.
3. 설치 안내가 뜨면 Xcode Command Line Tools를 설치합니다.
4. 설치 뒤 터미널을 닫았다가 다시 엽니다.
5. GitHub에 브라우저로 로그인해 둡니다.
6. `git push` 때 로그인 창이 뜨면 GitHub 계정을 선택하고 허용합니다.

맥북에서 자격 증명은 보통 키체인에 저장됩니다.  
처음 로그인에 성공하면 다음 `push`부터는 다시 로그인하지 않아도 되는 경우가 많습니다.

#### Mac 1단계: Git 설치 확인

터미널에 아래 명령어를 입력합니다.

```bash
git --version
```

버전이 나오면 준비된 것입니다.

예시:

```text
git version 2.45.0
```

버전이 나오지 않고 설치 안내 창이 뜨면 Xcode Command Line Tools 설치가 필요할 수 있습니다.  
안내 창이 나오면 설치를 진행한 뒤 터미널을 다시 열고 `git --version`을 한 번 더 입력합니다.

#### Mac 1-1단계: Git 사용자 이름과 이메일 설정

처음 commit을 하기 전에 한 번만 설정합니다.  
이 정보는 GitHub 로그인 비밀번호가 아니라, Git 기록에 남는 작성자 표시입니다.

```bash
git config --global user.name "내이름"
git config --global user.email "내이메일@example.com"
```

예시:

```bash
git config --global user.name "Minji Kim"
git config --global user.email "minji@example.com"
```

설정이 들어갔는지 확인합니다.

```bash
git config --global user.name
git config --global user.email
```

#### Mac 2단계: 포트폴리오 폴더로 이동

터미널에서 내 포트폴리오 폴더로 이동합니다.  
아래 경로는 예시입니다. 자기 컴퓨터에서 실제 폴더 위치에 맞게 바꿔야 합니다.

```bash
cd /Users/내사용자이름/Desktop/my-ai-portfolio
```

바탕화면에 `my-ai-portfolio` 폴더를 만들었다면 보통 이렇게 이동합니다.

```bash
cd ~/Desktop/my-ai-portfolio
```

폴더 이름에 띄어쓰기가 있으면 따옴표로 감싸면 안전합니다.

```bash
cd "$HOME/Desktop/my ai portfolio"
```

#### Mac 3단계: 파일 목록 확인

```bash
ls
```

아래 파일들이 보이면 좋습니다.

```text
index.html
style.css
script.js
club-logo.png
practice-guide.md
```

### 윈도우에서 Git 사용하기

윈도우에서는 방법이 두 가지 있습니다.

- 추천: `Git Bash` 사용
- 가능: `PowerShell` 사용

처음 배우는 학생에게는 `Git Bash`를 추천합니다.  
맥북과 비슷한 명령어를 쓸 수 있어서 수업 중 설명을 따라가기 쉽습니다.

#### Windows 0단계: 설치와 인증 환경 준비

윈도우에서 가장 중요한 준비는 Git for Windows 설치입니다.  
Git for Windows를 설치하면 Git Bash와 Git Credential Manager가 함께 준비됩니다.  
이 두 가지가 있어야 수업 중 `git push`를 했을 때 GitHub 로그인 창이 뜨고, 파일이 원격 저장소로 올라갈 가능성이 높습니다.

윈도우 사용자는 수업 전에 아래를 확인합니다.

1. Git for Windows를 설치합니다.
2. 설치 중 옵션은 처음에는 기본값 그대로 두는 것을 추천합니다.
3. 설치 화면에서 Git Credential Manager가 선택되어 있으면 그대로 둡니다.
4. 설치가 끝나면 열려 있던 PowerShell, 명령 프롬프트, VS Code를 모두 닫았다가 다시 엽니다.
5. 시작 메뉴에서 `Git Bash`를 검색해 열 수 있는지 확인합니다.
6. GitHub에 브라우저로 로그인해 둡니다.
7. `git push` 때 GitHub 로그인 창이 뜨면 브라우저에서 로그인하고 허용합니다.

처음 배우는 수업에서는 `명령 프롬프트`보다 `Git Bash`를 사용하는 것이 좋습니다.  
PowerShell도 가능하지만, 폴더 이동 명령어가 조금 달라져서 헷갈릴 수 있습니다.

#### Windows 1단계: Git 설치 확인

먼저 시작 메뉴에서 `Git Bash`를 검색해 열어 봅니다.  
Git Bash가 있다면 아래 명령어를 입력합니다.

```bash
git --version
```

버전이 나오면 준비된 것입니다.

```text
git version 2.45.0.windows.1
```

Git Bash가 없거나 `git` 명령어가 작동하지 않으면 Git for Windows를 설치해야 합니다.

설치할 때는 보통 기본값 그대로 `Next`를 눌러도 괜찮습니다.  
설치가 끝나면 Git Bash를 새로 열고 다시 확인합니다.

```bash
git --version
```

#### Windows 1-1단계: Git 사용자 이름과 이메일 설정

Git Bash에서 아래 명령어를 한 번만 실행합니다.

```bash
git config --global user.name "내이름"
git config --global user.email "내이메일@example.com"
```

예시:

```bash
git config --global user.name "Minji Kim"
git config --global user.email "minji@example.com"
```

설정 확인:

```bash
git config --global user.name
git config --global user.email
```

GitHub 계정 이메일과 똑같이 맞추면 나중에 GitHub에서 내 commit으로 잘 표시됩니다.

#### Windows 2단계: 포트폴리오 폴더로 이동하기

윈도우에서는 폴더 위치를 쓰는 방식이 조금 다릅니다.  
Git Bash를 쓰는지 PowerShell을 쓰는지에 따라 명령어가 달라질 수 있습니다.

Git Bash를 사용하는 경우, 바탕화면의 `my-ai-portfolio` 폴더로 이동하려면 이렇게 입력합니다.

```bash
cd ~/Desktop/my-ai-portfolio
```

PowerShell을 사용하는 경우에는 이렇게 입력합니다.

```powershell
cd "$HOME\Desktop\my-ai-portfolio"
```

만약 문서 폴더에 만들었다면 Git Bash에서는 이렇게 쓸 수 있습니다.

```bash
cd ~/Documents/my-ai-portfolio
```

PowerShell에서는 이렇게 쓸 수 있습니다.

```powershell
cd "$HOME\Documents\my-ai-portfolio"
```

폴더 이름에 띄어쓰기가 있으면 따옴표를 꼭 사용하세요.

```powershell
cd "$HOME\Desktop\my ai portfolio"
```

#### Windows 3단계: 파일 목록 확인

Git Bash를 사용하는 경우:

```bash
ls
```

PowerShell을 사용하는 경우:

```powershell
dir
```

아래 파일들이 보이면 좋습니다.

```text
index.html
style.css
script.js
club-logo.png
practice-guide.md
```

### 여기부터는 맥북과 윈도우가 거의 같습니다

이제부터는 현재 폴더에 들어온 뒤 실행하는 Git 명령어입니다.  
맥북 터미널, 윈도우 Git Bash, 윈도우 PowerShell에서 거의 똑같이 사용할 수 있습니다.

다만 윈도우 학생은 가능하면 Git Bash에서 계속 진행하는 것을 추천합니다.

### `push`가 성공하려면 먼저 확인할 것

아래 체크가 모두 되어 있어야 마지막 `git push`가 잘 됩니다.

- [ ] `git --version`이 정상 출력된다.
- [ ] `git config --global user.name`에 내 이름이 나온다.
- [ ] `git config --global user.email`에 내 이메일이 나온다.
- [ ] GitHub 웹사이트에 로그인할 수 있다.
- [ ] GitHub 이메일 인증이 끝났다.
- [ ] GitHub에 `my-ai-portfolio` 같은 빈 저장소를 만들었다.
- [ ] 저장소 주소가 `https://github.com/.../...git` 형태이다.
- [ ] 포트폴리오 파일 5개가 같은 폴더에 있다.
- [ ] 현재 터미널 위치가 그 포트폴리오 폴더이다.

현재 폴더가 맞는지 헷갈리면 파일 목록을 다시 봅니다.

맥북 또는 Git Bash:

```bash
ls
```

PowerShell:

```powershell
dir
```

`index.html`이 보이지 않으면 아직 포트폴리오 폴더에 들어오지 않은 것입니다.

### 공통 1단계: Git 기록 시작하기

처음 한 번만 실행합니다.

```bash
git init
```

이 말은 "이 폴더의 변화 기록을 시작할게"라는 뜻입니다.

### 공통 2단계: 현재 상태 확인하기

```bash
git status
```

Git이 "어떤 파일이 새로 생겼는지, 어떤 파일이 바뀌었는지" 알려 줍니다.  
선생님이 제출 전 검사표를 보는 것과 비슷합니다.

### 공통 3단계: 제출할 파일 고르기

모든 파일을 제출 봉투에 넣습니다.

```bash
git add .
```

`.`은 "현재 폴더의 파일들"이라는 뜻입니다.

조금 더 조심스럽게 하고 싶다면 파일을 하나씩 넣을 수도 있습니다.

```bash
git add index.html style.css script.js club-logo.png practice-guide.md
```

### 공통 4단계: 기록 사진 찍기

```bash
git commit -m "Add personal portfolio site"
```

`-m` 뒤의 문장은 기록 제목입니다.  
사진첩에 붙이는 제목표처럼 생각하면 됩니다.

좋은 커밋 메시지 예시:

```bash
git commit -m "Update portfolio notes section"
git commit -m "Add club logo image"
git commit -m "Change profile introduction"
```

너무 애매한 메시지는 피합니다.

```bash
git commit -m "fix"
git commit -m "asdf"
```

만약 처음 commit할 때 이름과 이메일을 알려 달라는 메시지가 나오면 아직 환경 세팅이 끝나지 않은 것입니다.  
아래 명령어를 실행한 뒤 다시 commit합니다.

```bash
git config --global user.name "내이름"
git config --global user.email "내이메일@example.com"
```

예시:

```bash
git config --global user.name "Minji Kim"
git config --global user.email "minji@example.com"
```

그다음 다시 commit합니다.

```bash
git commit -m "Add personal portfolio site"
```

### 공통 5단계: GitHub 저장소 만들기

GitHub 웹사이트에서 새 저장소를 만듭니다.

예시 저장소 이름:

```text
my-ai-portfolio
```

저장소를 만들면 GitHub가 주소를 보여 줍니다.

예시:

```text
https://github.com/내아이디/my-ai-portfolio.git
```

### 공통 6단계: 내 컴퓨터 폴더와 GitHub 저장소 연결하기

아래 명령에서 주소는 자기 저장소 주소로 바꿉니다.

```bash
git remote add origin https://github.com/내아이디/my-ai-portfolio.git
```

이 말은 "내 온라인 보관함 주소는 여기야"라고 알려 주는 것입니다.

연결이 잘 되었는지 확인합니다.

```bash
git remote -v
```

아래처럼 `origin` 주소가 보이면 연결된 것입니다.

```text
origin  https://github.com/내아이디/my-ai-portfolio.git (fetch)
origin  https://github.com/내아이디/my-ai-portfolio.git (push)
```

### 공통 7단계: 기본 가지 이름을 main으로 맞추기

```bash
git branch -M main
```

GitHub Pages에서 보통 `main` 가지를 사용하므로 이렇게 맞춰 둡니다.

### 공통 8단계: GitHub로 보내기

```bash
git push -u origin main
```

처음 보낼 때는 GitHub 로그인이 필요할 수 있습니다.  
맥북에서는 브라우저 로그인 창이나 키체인 확인 창이 뜰 수 있습니다.  
윈도우에서는 브라우저 로그인 창이나 Git Credential Manager 창이 뜰 수 있습니다.  
비밀번호를 터미널에 직접 입력하는 방식이 아니라, GitHub 로그인 화면이 열릴 수 있다는 뜻입니다.

로그인 창이 뜨면 아래 순서대로 진행합니다.

1. 브라우저가 열리면 GitHub 계정으로 로그인합니다.
2. `Authorize Git Credential Manager` 또는 비슷한 허용 버튼이 나오면 허용합니다.
3. 2단계 인증을 쓰는 계정이면 인증을 완료합니다.
4. 터미널로 돌아와서 `push`가 끝나는지 기다립니다.

성공하면 보통 아래와 비슷한 문장이 보입니다.

```text
Writing objects: 100% ...
To https://github.com/내아이디/my-ai-portfolio.git
 * [new branch]      main -> main
```

성공하면 내 컴퓨터의 기록이 GitHub 저장소에 올라갑니다.

정말 올라갔는지 확인하려면 GitHub 저장소 페이지를 새로고침합니다.  
`index.html`, `style.css`, `script.js`, `club-logo.png`, `practice-guide.md`가 저장소 화면에 보이면 성공입니다.

다음부터는 보통 이렇게 반복합니다.

```bash
git status
git add .
git commit -m "Update portfolio"
git push
```

외우기 어렵다면 이렇게 기억하세요.

```text
상태 보기 -> 봉투에 넣기 -> 사진 찍기 -> 온라인으로 보내기
```

명령어로 쓰면:

```bash
git status
git add .
git commit -m "작업 내용"
git push
```

### 운영체제별로 기억할 차이 정리

| 상황 | 맥북 | 윈도우 Git Bash | 윈도우 PowerShell |
| --- | --- | --- | --- |
| 프로그램 열기 | 터미널 | Git Bash | PowerShell |
| 바탕화면 이동 | `cd ~/Desktop/my-ai-portfolio` | `cd ~/Desktop/my-ai-portfolio` | `cd "$HOME\Desktop\my-ai-portfolio"` |
| 파일 목록 보기 | `ls` | `ls` | `dir` |
| Git 버전 확인 | `git --version` | `git --version` | `git --version` |
| 사용자 설정 확인 | `git config --global user.email` | `git config --global user.email` | `git config --global user.email` |
| 인증 저장 위치 | 키체인 | Windows Credential Manager | Windows Credential Manager |
| Git 명령어 | 대부분 동일 | 대부분 동일 | 대부분 동일 |

오늘 수업에서 헷갈리면 이 표만 보고 따라가도 됩니다.

## 5. 자주 생기는 문제

### 맥북에서 `git`을 입력했더니 설치 창이 떠요

Git이 아직 준비되지 않았다는 뜻입니다.  
Xcode Command Line Tools 설치 안내가 뜨면 설치를 진행합니다.  
설치가 끝난 뒤 터미널을 완전히 닫았다가 다시 열고 확인합니다.

```bash
git --version
```

### 윈도우에서 `'git'은 내부 또는 외부 명령...`이라고 나와요

Git이 설치되지 않았거나, 터미널이 Git을 찾지 못한다는 뜻입니다.

해결 방법:

1. Git for Windows를 설치합니다.
2. 설치 후 열려 있던 PowerShell이나 Git Bash를 닫습니다.
3. Git Bash를 새로 엽니다.
4. 다시 확인합니다.

```bash
git --version
```

처음 실습에서는 PowerShell보다 Git Bash를 쓰는 것이 더 쉽습니다.

### 폴더로 이동했는데 `No such file or directory` 또는 `Cannot find path`라고 나와요

폴더 주소가 틀렸다는 뜻입니다.

확인할 것:

- 바탕화면에 실제로 `my-ai-portfolio` 폴더가 있는가?
- 폴더 이름에 띄어쓰기가 있는데 따옴표를 빠뜨리지 않았는가?
- 맥북 명령어를 윈도우 PowerShell에 그대로 넣고 있지는 않은가?

맥북 또는 Git Bash 예시:

```bash
cd ~/Desktop/my-ai-portfolio
```

윈도우 PowerShell 예시:

```powershell
cd "$HOME\Desktop\my-ai-portfolio"
```

### `nothing to commit`이라고 나와요

바뀐 파일이 없다는 뜻입니다.  
이미 사진을 찍어 둔 상태와 지금 상태가 같다는 말입니다.

### `remote origin already exists`라고 나와요

이미 GitHub 주소가 연결되어 있다는 뜻입니다.

현재 연결된 주소를 확인합니다.

```bash
git remote -v
```

주소를 바꿔야 한다면 이렇게 합니다.

```bash
git remote set-url origin https://github.com/내아이디/my-ai-portfolio.git
```

### `git push`를 했는데 로그인 창이 안 떠요

Git Credential Manager가 제대로 준비되지 않았거나, 예전에 잘못된 로그인 정보가 저장되어 있을 수 있습니다.

먼저 원격 주소가 HTTPS인지 확인합니다.

```bash
git remote -v
```

주소가 아래처럼 `https://`로 시작해야 합니다.

```text
https://github.com/내아이디/my-ai-portfolio.git
```

주소가 `git@github.com:...`처럼 시작하면 SSH 주소입니다.  
처음 수업에서는 HTTPS 주소로 바꾸는 것이 쉽습니다.

```bash
git remote set-url origin https://github.com/내아이디/my-ai-portfolio.git
```

그다음 다시 push합니다.

```bash
git push -u origin main
```

### `Authentication failed` 또는 `Support for password authentication was removed`라고 나와요

GitHub 비밀번호를 터미널에 직접 입력해서는 `push`가 되지 않는다는 뜻입니다.  
Git Credential Manager 로그인 창을 사용하거나, 선생님 안내에 따라 Personal Access Token을 사용해야 합니다.

수업에서는 먼저 아래 순서로 해결합니다.

1. GitHub 웹사이트에 브라우저로 로그인합니다.
2. 터미널에서 원격 주소가 HTTPS인지 확인합니다.
3. 다시 `git push -u origin main`을 입력합니다.
4. 로그인 창이 뜨면 GitHub 로그인을 허용합니다.

윈도우에서 예전 비밀번호가 저장되어 계속 실패한다면 `Windows 자격 증명 관리자`에서 GitHub 관련 항목을 지운 뒤 다시 시도할 수 있습니다.  
맥북에서는 `키체인 접근`에서 GitHub 관련 항목을 확인해야 할 수 있습니다.  
이 단계는 계정 정보와 관련되므로 수업에서는 선생님과 함께 진행하는 것이 안전합니다.

### `Repository not found`라고 나와요

GitHub 저장소 주소가 틀렸거나, 저장소가 아직 만들어지지 않았거나, 로그인한 계정이 그 저장소에 접근 권한이 없다는 뜻입니다.

확인할 것:

- GitHub 웹사이트에서 저장소가 실제로 열리는가?
- 저장소 주소의 아이디와 저장소 이름에 오타가 없는가?
- 터미널의 원격 주소가 저장소 주소와 같은가?

```bash
git remote -v
```

주소가 틀렸다면 다시 설정합니다.

```bash
git remote set-url origin https://github.com/내아이디/my-ai-portfolio.git
```

### `Updates were rejected`라고 나와요

GitHub 저장소에 이미 README 같은 파일이 있어서 내 컴퓨터 기록과 GitHub 기록이 서로 다를 때 나올 수 있습니다.

처음 수업에서는 가장 쉬운 해결 방법이 있습니다.

- GitHub에서 새 저장소를 만들 때 README를 만들지 않습니다.
- 이미 README를 만든 저장소라면, 새 저장소를 다시 만들거나 선생님 안내를 받아 `git pull`을 먼저 해야 합니다.

초보 실습에서는 충돌 해결까지 들어가면 복잡해지므로, 빈 저장소로 시작하는 것을 추천합니다.

### `src refspec main does not match any`라고 나와요

아직 commit이 없거나 branch 이름이 맞지 않을 때 나올 수 있습니다.

아래 순서대로 확인합니다.

```bash
git status
git add .
git commit -m "Add personal portfolio site"
git branch -M main
git push -u origin main
```

`git commit`에서 이름과 이메일을 설정하라는 메시지가 나오면 먼저 `git config --global user.name`, `git config --global user.email`을 설정해야 합니다.

### GitHub Pages 주소가 404로 나와요

가게 문을 열었는데 아직 간판이 붙는 중일 수 있습니다.  
몇 분 기다렸다가 다시 확인합니다.

그래도 안 되면:

- `index.html`이 저장소 첫 화면에 있는지 확인합니다.
- Pages 설정이 `main`과 `/(root)`인지 확인합니다.
- 파일 이름에 대문자나 오타가 없는지 확인합니다.

### 로고 이미지가 안 보여요

`index.html`과 같은 위치에 `club-logo.png`가 있어야 합니다.

좋은 구조:

```text
my-ai-portfolio/
  index.html
  style.css
  script.js
  club-logo.png
  practice-guide.md
```

잘못된 구조:

```text
my-ai-portfolio/
  index.html
  images/
    club-logo.png
```

이미지를 `images` 폴더에 넣고 싶다면 HTML의 `src`도 바꿔야 합니다.

```html
src="images/club-logo.png"
```

## 6. 제출 전 마지막 점검표

- [ ] 내 이름과 자기소개로 바꾸었다.
- [ ] 관심 분야와 프로젝트 카드를 내 활동에 맞게 바꾸었다.
- [ ] 동아리 로고가 보인다.
- [ ] 포트폴리오 기록에 새 메모를 추가해 보았다.
- [ ] CodePen에서 HTML, CSS, JS가 작동하는지 확인했다.
- [ ] 맥북 또는 윈도우 중 내 컴퓨터에 맞는 Git 안내를 따라 했다.
- [ ] GitHub 저장소에 파일을 올렸다.
- [ ] GitHub Pages 주소로 접속해 보았다.
- [ ] 휴대폰 화면에서도 글자가 겹치지 않는지 확인했다.

## 7. 참고 공식 문서

- Git 설치 공식 가이드: <https://github.com/git-guides/install-git>
- GitHub 자격 증명 저장 공식 문서: <https://docs.github.com/en/get-started/git-basics/caching-your-github-credentials-in-git>
- Git Credential Manager 설치 문서: <https://github.com/git-ecosystem/git-credential-manager/blob/main/docs/install.md>
- Personal Access Token 공식 문서: <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens>
- GitHub Pages 공식 문서: <https://docs.github.com/pages>
- GitHub 저장소에 파일 추가하기: <https://docs.github.com/repositories/working-with-files/managing-files/adding-a-file-to-a-repository>
- GitHub에 원격 저장소 추가하기: <https://docs.github.com/get-started/git-basics/managing-remote-repositories>
- CodePen 공식 문서: <https://blog.codepen.io/documentation/>
