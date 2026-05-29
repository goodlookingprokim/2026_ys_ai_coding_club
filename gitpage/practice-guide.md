# AI창의융합코딩연구반 개인 포트폴리오 실습 가이드

오늘 실습은 아래 순서로 진행합니다.

1. CodePen에 완성된 코드를 먼저 붙여 넣고 화면을 확인합니다.
2. 필요한 부분을 자기 정보와 자기 활동으로 수정합니다.
3. CodePen에서 결과물을 내려받아 내 컴퓨터 폴더에 정리합니다.
4. GitHub 사이트에 파일을 업로드합니다.
5. GitHub Pages 설정을 켜서 인터넷 주소로 게시합니다.
6. 더 배우고 싶은 학생은 Git으로 커밋하고 GitHub로 푸시하는 방법까지 연습합니다.

먼저 큰 그림을 기억하세요.

- CodePen은 연습장입니다. 코드를 붙여 넣자마자 화면을 볼 수 있습니다.
- GitHub는 보관함입니다. 내 파일을 인터넷에 올려 보관합니다.
- GitHub Pages는 전시대입니다. 보관한 파일을 웹사이트 주소로 보여 줍니다.
- Git은 사진첩입니다. 파일이 바뀐 순간을 기록해 둡니다.

## 1. 준비물 확인하기

오늘 사용하는 파일은 다음과 같습니다.

- `index.html`: 화면의 글과 구조
- `style.css`: 색, 크기, 카드 모양
- `script.js`: 프로젝트 카드, 필터 버튼, 포트폴리오 기록 기능
- `club-logo.png`: 동아리 로고 이미지
- `practice-guide.md`: 지금 읽고 있는 실습 안내 파일

비유하면 이렇습니다.

- `index.html`: 집의 방 배치도
- `style.css`: 벽지, 조명, 가구 색
- `script.js`: 스위치와 리모컨
- `club-logo.png`: 현관 간판

## 2. CodePen에 완성된 코드 먼저 붙여 넣기

처음부터 코드를 고치려고 하면 어디가 맞고 어디가 틀린지 알기 어렵습니다.  
먼저 완성된 코드를 CodePen에 그대로 넣고 화면이 나오는지 봅니다.

### 2-1. 새 Pen 만들기

1. CodePen에 로그인합니다.
2. `Create` 또는 `New Pen`을 눌러 새 Pen을 만듭니다.
3. 화면에 HTML, CSS, JS 패널이 보이는지 확인합니다.

CodePen의 세 칸은 도시락 칸처럼 나뉘어 있습니다.

- HTML 칸: 화면에 놓을 재료
- CSS 칸: 재료를 예쁘게 담는 방법
- JS 칸: 버튼을 눌렀을 때 움직이는 방법

### 2-2. HTML 패널에 붙여 넣기

`index.html`에서 `<body>` 안쪽 내용을 HTML 패널에 붙여 넣습니다.

복사 범위:

- 시작: `<header class="site-header">`
- 끝: `<footer class="site-footer">...</footer>`

CodePen HTML 패널에는 보통 아래 줄들은 넣지 않습니다.

```html
<!DOCTYPE html>
<html>
<head>
<body>
<link rel="stylesheet" href="style.css" />
<script src="script.js"></script>
```

왜냐하면 CodePen이 이미 보이지 않는 곳에서 기본 HTML 틀을 만들어 주기 때문입니다.  
도시락통은 CodePen이 준비해 주고, 우리는 도시락 안에 들어갈 내용만 넣는다고 생각하면 됩니다.

### 2-3. CSS 패널에 붙여 넣기

`style.css` 파일 전체를 CSS 패널에 붙여 넣습니다.

`style.css`는 사이트의 옷입니다.  
이 파일을 넣어야 카드, 색상, 여백, 모바일 화면 모양이 제대로 보입니다.

### 2-4. JS 패널에 붙여 넣기

`script.js` 파일 전체를 JS 패널에 붙여 넣습니다.

이 파일을 넣어야 아래 기능이 작동합니다.

- 동아리 활동 목록 자동 표시
- 프로젝트 카드 자동 표시
- `전체`, `웹`, `AI`, `데이터` 필터 버튼
- 포트폴리오 기록 추가
- 기록을 브라우저에 저장하기

### 2-5. 동아리 로고는 어떻게 하나요?

이 사이트는 `club-logo.png`를 사용합니다.  
GitHub Pages에서는 `index.html`과 같은 폴더에 `club-logo.png`를 올리면 바로 보입니다.

CodePen에서는 이미지 파일 처리가 계정 상태에 따라 다를 수 있습니다.

수업 중에는 이렇게 진행하면 됩니다.

1. 처음에는 로고가 완벽하게 안 보여도 HTML, CSS, JS가 작동하는지 먼저 확인합니다.
2. CodePen에서 이미지 업로드 기능을 사용할 수 있으면 `club-logo.png`를 업로드합니다.
3. 업로드한 이미지 주소를 복사합니다.
4. HTML의 `src="club-logo.png"` 부분을 업로드한 이미지 주소로 바꿉니다.

예시:

```html
<img class="club-logo-image" src="club-logo.png" alt="2026 AI창의융합 코딩연구반 로고" />
```

를 아래처럼 바꿀 수 있습니다.

```html
<img class="club-logo-image" src="이미지주소" alt="2026 AI창의융합 코딩연구반 로고" />
```

이미지가 아직 없어도 너무 걱정하지 마세요.  
이 포트폴리오에는 이미지가 없을 때 보이는 대체 박스가 준비되어 있습니다.

### 2-6. 먼저 확인할 것

CodePen 결과 화면에서 아래를 확인합니다.

- 첫 화면 큰 제목이 보이는가?
- 프로필 카드가 보이는가?
- 동아리 로고 영역이 보이는가?
- 동아리 활동 목록이 보이는가?
- 프로젝트 카드가 보이는가?
- 필터 버튼을 누르면 카드가 바뀌는가?
- 포트폴리오 기록에 메모를 쓰면 바로 목록에 보이는가?

여기까지 되면 "기본 자동차에 시동이 걸린 상태"입니다.  
이제 색을 바꾸고, 이름을 바꾸고, 프로젝트 내용을 바꾸면 됩니다.

## 3. 필요한 부분 수정하기

오늘의 목표는 예쁜 예시 페이지를 그대로 제출하는 것이 아닙니다.  
내가 수행한 활동이 드러나는 개인 포트폴리오로 바꾸는 것입니다.

코드 안의 `수정:` 주석을 먼저 찾으세요.  
이 주석은 "여기는 학생이 바꿔도 되는 곳"이라는 작은 포스트잇입니다.

### 3-1. 수정할 때 지키는 쉬운 규칙

- 따옴표 `" "` 안의 글을 바꿀 때는 따옴표를 지우지 않습니다.
- `<h1>내용</h1>`처럼 태그 사이의 글을 바꿀 때는 태그는 그대로 두고 글만 바꿉니다.
- JavaScript에서 `{}`, `[]`, `,`는 중요합니다. 글만 바꾸고 기호는 함부로 지우지 않습니다.
- 한 번에 전부 바꾸지 말고 2~3곳을 바꾼 뒤 결과 화면을 확인합니다.

수정은 김밥 속 재료를 바꾸는 일과 비슷합니다.  
김, 밥, 말아 놓은 모양은 유지하고 안쪽 재료만 내 취향으로 바꾸는 것입니다.

### 3-2. `index.html`에서 바꿀 것

`index.html`은 화면에 보이는 글을 담당합니다.

바꾸기 좋은 곳:

- 브라우저 제목
- 왼쪽 위 로고 글자
- 첫 화면 큰 제목
- 자기소개 문장
- 이름과 학년
- 관심 분야
- 관심 키워드
- 배운 점
- 이메일과 GitHub 링크
- 맨 아래 문구

예시 1: 이름 바꾸기

```html
<h2>홍길동</h2>
```

```html
<h2>김민지</h2>
```

예시 2: 큰 제목 바꾸기

```html
<h1 id="hero-title">코딩으로 생각을 만들고, AI로 가능성을 넓힙니다.</h1>
```

```html
<h1 id="hero-title">AI와 코딩으로 나의 아이디어를 직접 만들어 봅니다.</h1>
```

예시 3: 자기소개 문장 바꾸기

```html
안녕하세요. 저는 문제를 관찰하고, 작은 아이디어를 코드로 구현하는 과정을 좋아하는 학생입니다.
```

```html
안녕하세요. 저는 생활 속 불편함을 찾아보고, AI와 웹 기술로 해결 방법을 만들어 보는 학생입니다.
```

예시 4: GitHub 주소 바꾸기

```html
<a href="https://github.com/" target="_blank" rel="noreferrer">GitHub</a>
```

```html
<a href="https://github.com/my-id" target="_blank" rel="noreferrer">GitHub</a>
```

### 3-3. `script.js`에서 바꿀 것

`script.js`는 화면에 자동으로 만들어지는 목록을 담당합니다.

바꾸기 좋은 곳:

- `activityData`: 동아리 활동 기록
- `projectData`: 프로젝트 카드
- `starterNoteData`: 처음 보이는 예시 기록

예시 1: 동아리 활동 바꾸기

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

예시 2: 프로젝트 카드 바꾸기

```js
{
  title: "나를 소개하는 웹 페이지",
  description: "HTML과 CSS를 사용해 자기소개, 관심 분야, 목표를 정리한 첫 페이지입니다.",
  category: "web",
  icon: "WEB",
  tags: ["HTML", "CSS", "기초"],
}
```

```js
{
  title: "학교생활 도우미 웹 페이지",
  description: "학교생활에서 자주 확인하는 일정과 준비물을 한 화면에 정리했습니다.",
  category: "web",
  icon: "WEB",
  tags: ["HTML", "CSS", "학교생활"],
}
```

`category`는 필터 버튼과 연결됩니다.

- `web`: 웹 버튼을 눌렀을 때 보임
- `ai`: AI 버튼을 눌렀을 때 보임
- `data`: 데이터 버튼을 눌렀을 때 보임

예시 3: 처음 보이는 기록 바꾸기

```js
title: "첫 포트폴리오 구조 만들기",
content: "HTML 섹션을 나누고 자기소개, 활동, 프로젝트 영역을 만들었습니다.",
```

```js
title: "프로젝트 아이디어 정리",
content: "내가 해결하고 싶은 문제를 적고 필요한 기능을 간단히 목록으로 만들었습니다.",
```

아래 코드는 수업 중에는 바꾸지 않는 것이 좋습니다.

```js
const notesStorageKey = "ysPortfolioNotes";
```

이 이름은 브라우저가 포트폴리오 기록을 저장할 때 쓰는 이름입니다.  
사물함 이름표를 마음대로 바꾸면 이전에 넣어 둔 물건을 찾기 어려운 것과 비슷합니다.

### 3-4. `style.css`에서 바꿀 것

`style.css`는 사이트 분위기를 담당합니다.  
처음에는 전체 구조보다 색상 변수만 바꿔 보는 것을 추천합니다.

예시 1: 대표 색 바꾸기

```css
--color-primary: #0f766e;
```

```css
--color-primary: #2563eb;
```

예시 2: 포인트 색 바꾸기

```css
--color-warm: #f6c453;
```

```css
--color-warm: #f9a8d4;
```

예시 3: 카드 둥근 정도 바꾸기

```css
--radius: 8px;
```

```css
--radius: 4px;
```

숫자가 작으면 더 각진 카드가 되고, 숫자가 크면 더 둥근 카드가 됩니다.

### 3-5. 포트폴리오 기록 남기기

사이트 중간의 `포트폴리오 기록` 섹션에는 오늘 한 일을 바로 적을 수 있습니다.

예시:

- 기록 제목: `첫 웹 페이지 완성`
- 활동 종류: `실습`
- 기록 내용: `HTML로 자기소개 영역을 만들고 CSS로 카드 모양을 꾸몄다.`

`기록 추가` 버튼을 누르면 아래 목록에 바로 보입니다.

중요한 점:

- 복잡한 데이터베이스를 쓰지 않습니다.
- 현재 브라우저 안에 저장됩니다.
- 같은 컴퓨터, 같은 브라우저에서는 새로고침해도 남아 있습니다.
- 브라우저 기록을 지우거나 다른 컴퓨터로 가면 사라질 수 있습니다.

이 기록은 책상 위 개인 메모지와 비슷합니다.  
내 책상에는 남아 있지만 친구 책상이나 학교 서버에 자동으로 붙는 메모는 아닙니다.

기록으로 남기기 좋은 문장:

- `HTML로 자기소개 영역을 만들고 제목과 문단 태그의 차이를 알게 되었다.`
- `CSS 색상 변수를 바꾸어 사이트 분위기가 어떻게 달라지는지 확인했다.`
- `프로젝트 카드 내용을 내 활동에 맞게 수정했다.`
- `AI에게 질문할 때 조건을 자세히 적으면 답변이 더 정확해진다는 것을 배웠다.`
- `GitHub Pages에 파일을 올리고 인터넷 주소로 접속해 보았다.`

## 4. CodePen에서 내 컴퓨터로 다운로드하기

CodePen에서 수정이 끝났다면 결과물을 내 컴퓨터로 내려받습니다.

공책에 연습한 내용을 사진으로 남겨 가방에 넣는 과정이라고 생각하면 됩니다.

### 4-1. CodePen 저장하기

1. CodePen에서 `Save`를 누릅니다.
2. 제목을 정합니다.
   - 예: `김민지 AI 포트폴리오`
3. 결과 화면이 제대로 보이는지 다시 확인합니다.

### 4-2. Export .zip으로 내려받기

1. CodePen 편집 화면에서 `Export` 메뉴를 찾습니다.
2. `Export .zip`을 선택합니다.
3. `.zip` 파일이 다운로드됩니다.
4. 다운로드한 `.zip` 파일을 압축 해제합니다.

CodePen에서 내려받은 폴더에는 보통 이런 폴더가 들어 있습니다.

- `src`: 내가 CodePen 패널에 입력한 원본 코드
- `dist`: 브라우저에서 바로 볼 수 있게 만들어진 결과물

오늘처럼 HTML, CSS, JavaScript만 쓰는 실습에서는 GitHub Pages에 올릴 때 `dist` 폴더 안 파일을 사용하면 쉽습니다.

### 4-3. 로컬 게시 폴더 정리하기

내 컴퓨터에 새 폴더를 하나 만듭니다.

예시 이름:

```text
my-ai-portfolio
```

그 안에 GitHub Pages에 올릴 파일을 모읍니다.

기본 구조:

```text
my-ai-portfolio/
  index.html
  style.css
  script.js
  club-logo.png
  practice-guide.md
```

CodePen에서 내려받은 `dist` 폴더를 사용할 때는 `dist` 안의 파일을 확인합니다.  
로고가 보이려면 `club-logo.png`도 같은 폴더에 넣어야 합니다.

파일 이름은 가게 간판과 같습니다.  
`index.html`을 `Index.html`이나 `main.html`로 바꾸면 GitHub Pages가 첫 화면을 바로 찾지 못할 수 있습니다.

## 5. GitHub 사이트에 업로드하고 Pages로 게시하기

GitHub 웹사이트만 사용해서 게시하는 방법입니다.  
터미널이 아직 익숙하지 않은 학생은 이 방법으로 먼저 성공해 봅니다.

### 5-1. GitHub 저장소 만들기

1. GitHub에 로그인합니다.
2. 오른쪽 위 `+` 버튼을 누릅니다.
3. `New repository`를 선택합니다.
4. 저장소 이름을 정합니다.
   - 예: `my-ai-portfolio`
5. 수업용이면 `Public`으로 둡니다.
6. `Create repository`를 누릅니다.

저장소는 인터넷 보관함입니다.  
오늘 만든 파일을 넣어 둘 상자라고 생각하면 됩니다.

### 5-2. 파일 업로드하기

1. 새 저장소 화면에서 `Add file`을 누릅니다.
2. `Upload files`를 선택합니다.
3. 로컬 게시 폴더 안의 파일을 끌어다 놓습니다.
4. 아래 파일이 들어갔는지 확인합니다.
   - `index.html`
   - `style.css`
   - `script.js`
   - `club-logo.png`
   - `practice-guide.md`
5. 아래쪽 `Commit changes`를 누릅니다.
   - 화면에 `Propose changes`라고 보이면 그 버튼을 눌러도 됩니다.

`Commit changes`는 현재 파일 상태를 사진처럼 찍어 저장하는 일입니다.

### 5-3. GitHub Pages 켜기

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

처음에는 바로 보이지 않을 수 있습니다.  
인터넷 게시판에 작품을 붙인 뒤 간판이 켜지는 데 시간이 조금 걸리는 것과 비슷합니다.

### 5-4. 게시 후 확인할 것

- 주소로 접속했을 때 첫 화면이 보이는가?
- 동아리 로고가 보이는가?
- CSS가 적용되어 카드와 색상이 제대로 보이는가?
- 필터 버튼이 작동하는가?
- 포트폴리오 기록에 메모를 추가할 수 있는가?
- 휴대폰에서도 글자가 겹치지 않는가?

### 5-5. 안 보일 때 확인하기

GitHub Pages 주소가 404로 보이면 아래를 확인합니다.

- `index.html`이 저장소 첫 화면에 있는가?
- 파일 이름이 정확히 `index.html`인가?
- Pages 설정이 `main`, `/(root)`인가?
- `style.css`, `script.js`, `club-logo.png`가 `index.html`과 같은 위치에 있는가?
- 방금 게시했다면 몇 분 더 기다려 보았는가?

로고가 안 보이면 아래를 확인합니다.

- 파일 이름이 정확히 `club-logo.png`인가?
- `club-logo.png`가 `index.html`과 같은 폴더에 있는가?
- HTML의 `src`가 `club-logo.png`로 되어 있는가?

## 6. 더 깊게 배우기: Git과 GitHub로 커밋하고 푸시하기

여기부터는 개발자들이 자주 쓰는 방식입니다.  
GitHub 웹사이트에 직접 업로드하는 대신, 내 컴퓨터에서 명령어로 파일을 보냅니다.

쉬운 비유:

- 작업 폴더: 내 책상
- `git status`: 책상 위 상태 확인
- `git add`: 제출할 종이를 봉투에 넣기
- `git commit`: 봉투에 제목을 쓰고 사진 찍기
- `git push`: 온라인 보관함으로 보내기

### 6-1. Git 설치 확인

터미널을 열고 입력합니다.

```bash
git --version
```

버전이 나오면 준비된 것입니다.

### 6-2. 포트폴리오 폴더로 이동

예시:

```bash
cd ~/Desktop/my-ai-portfolio
```

현재 실습 폴더를 그대로 쓴다면:

```bash
cd /Users/jaiclass/Documents/tmp/YS_Coding_Club
```

파일 확인:

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

### 6-3. Git 기록 시작

처음 한 번만 실행합니다.

```bash
git init
```

"이 폴더의 변화 기록을 시작할게"라는 뜻입니다.

### 6-4. 상태 확인

```bash
git status
```

Git이 어떤 파일이 새로 생겼고 어떤 파일이 바뀌었는지 알려 줍니다.

### 6-5. 제출 봉투에 넣기

```bash
git add .
```

`.`은 현재 폴더의 파일들을 뜻합니다.

조금 더 조심스럽게 하고 싶다면 파일을 하나씩 넣습니다.

```bash
git add index.html style.css script.js club-logo.png practice-guide.md
```

### 6-6. 사진 찍듯이 기록하기

```bash
git commit -m "Add personal portfolio site"
```

`-m` 뒤의 문장은 기록 제목입니다.

좋은 제목 예시:

```bash
git commit -m "Update portfolio introduction"
git commit -m "Add portfolio notes section"
git commit -m "Add club logo image"
```

너무 짧아서 의미를 알기 어려운 제목은 피합니다.

```bash
git commit -m "fix"
git commit -m "asdf"
```

### 6-7. GitHub 저장소와 연결

GitHub에서 새 저장소를 만든 뒤 주소를 복사합니다.

예시 주소:

```text
https://github.com/내아이디/my-ai-portfolio.git
```

터미널에서 연결합니다.

```bash
git remote add origin https://github.com/내아이디/my-ai-portfolio.git
```

이 말은 "온라인 보관함 주소는 여기야"라고 알려 주는 것입니다.

이미 연결된 주소가 있다면 확인합니다.

```bash
git remote -v
```

주소를 바꾸어야 한다면:

```bash
git remote set-url origin https://github.com/내아이디/my-ai-portfolio.git
```

### 6-8. 가지 이름을 main으로 맞추기

```bash
git branch -M main
```

GitHub Pages에서 `main`을 쓰기 쉽게 맞춰 둡니다.

### 6-9. GitHub로 보내기

```bash
git push -u origin main
```

성공하면 내 컴퓨터의 기록이 GitHub 저장소에 올라갑니다.

다음부터는 보통 아래 순서를 반복합니다.

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

## 7. 마지막 점검표

- [ ] CodePen에 완성 코드를 먼저 붙여 넣고 화면을 확인했다.
- [ ] 내 이름, 자기소개, 관심 분야를 바꾸었다.
- [ ] 프로젝트 카드와 동아리 활동을 내 활동에 맞게 수정했다.
- [ ] 포트폴리오 기록에 새 메모를 추가해 보았다.
- [ ] CodePen에서 `.zip` 파일을 다운로드했다.
- [ ] 내 컴퓨터 로컬 폴더에 파일을 정리했다.
- [ ] GitHub 저장소에 파일을 업로드했다.
- [ ] GitHub Pages 설정을 켰다.
- [ ] Pages 주소로 접속해 보았다.
- [ ] 더 배우는 단계로 Git 커밋과 푸시를 연습했다.

## 8. 참고 공식 문서

- GitHub Pages 공식 문서: <https://docs.github.com/pages>
- GitHub 저장소에 파일 추가하기: <https://docs.github.com/repositories/working-with-files/managing-files/adding-a-file-to-a-repository>
- GitHub 원격 저장소 관리하기: <https://docs.github.com/get-started/git-basics/managing-remote-repositories>
- CodePen 공식 문서: <https://blog.codepen.io/documentation/>
- CodePen Export 공식 문서: <https://blog.codepen.io/docs/pens/exporting/>

