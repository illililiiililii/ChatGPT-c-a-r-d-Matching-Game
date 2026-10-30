# 야식 창고 털기 🍪

카드 속 간식의 위치를 기억하고 같은 간식 두 장을 찾는 작은 기억력 게임입니다. 설치나 빌드 없이 브라우저에서 실행할 수 있습니다.

## 바로 실행하기

1. 이 저장소의 파일을 내려받습니다. GitHub에서는 **Code → Download ZIP**을 누른 뒤 압축을 풀면 됩니다.
2. `index.html`을 더블클릭해 브라우저로 엽니다.
3. 카드 두 장을 눌러 같은 간식을 찾아보세요!

게임을 실행하는 데 Node.js, Python, API 키, 로그인이 필요하지 않습니다.

## 게임 방법

- 카드는 총 12장이고, 같은 간식이 2장씩 있습니다.
- 두 장이 같으면 간식을 확보합니다. 다른 간식이면 약 0.9초 뒤 다시 가려집니다.
- 카드 두 장을 고를 때마다 시도 횟수가 1회 늘어납니다.
- 6쌍을 전부 찾으면 성공입니다. 적은 시도 횟수로 완료해보세요.
- **다시 섞기**를 누르면 새 판을 시작합니다.
- 찾은 간식, 시도 횟수, 최고 기록을 표시합니다. 최고 기록은 완료한 게임 중 가장 적은 시도 횟수입니다.

키보드로는 `Tab`으로 카드를 선택하고 `Enter` 또는 `Space`로 뒤집을 수 있습니다.

## 포함된 파일

```text
snack-match/
├── index.html   # 브라우저에서 실행하는 게임
├── README.md    # 실행·업로드·공개 방법
└── .nojekyll    # GitHub Pages에서 정적 파일로 배포하기 위한 파일
```

`index.html` 안에 화면 스타일과 게임 코드가 포함되어 있습니다. 게임만 실행하려면 이 파일 하나면 됩니다.

## GitHub에 업로드하기 — 웹에서

1. GitHub에 로그인하고 새 저장소를 만듭니다. 이름은 예를 들어 `snack-match`로 정합니다.
2. 공개 배포를 간단히 따라 하려면 **Public** 저장소로 만듭니다.
3. 빈 저장소 화면의 **uploading an existing file**, 또는 기존 저장소의 **Add file → Upload files**를 선택합니다.
4. 이 폴더 안의 `index.html`, `README.md`, `.nojekyll`을 업로드합니다.
5. 커밋 메시지를 적고 **Commit changes**를 누릅니다.

**중요:** `snack-match` 폴더째 넣지 말고, 그 안의 파일을 저장소 최상위에 넣으세요. 저장소를 열었을 때 `index.html`과 `README.md`가 바로 보여야 합니다. `.nojekyll`은 내용이 없는 파일이며, 숨김 파일 표시 설정에 따라 보이지 않을 수 있습니다.

이미 같은 이름의 파일이 있는 저장소라면 덮어쓸 파일을 먼저 확인하세요. 처음이라면 새 저장소 사용을 권합니다.

## GitHub Pages로 게임 공개하기

파일 업로드를 마친 다음 설정합니다.

1. GitHub 저장소에서 **Settings → Pages**로 이동합니다.
2. **Build and deployment**의 **Source**를 **Deploy from a branch**로 선택합니다.
3. **Branch**는 파일을 올린 브랜치(보통 `main`), 폴더는 **/(root)**로 선택합니다.
4. **Save**를 누릅니다.
5. 배포가 완료되면 Pages 설정에 표시되는 **Visit site**로 게임을 엽니다.

일반적인 프로젝트 저장소의 주소 형식은 다음과 같습니다. 아래 주소는 예시이므로 본인의 사용자명과 저장소 이름으로 바꾸세요.

```text
https://YOUR-USERNAME.github.io/snack-match/
```

이 주소를 친구에게 보내면 브라우저에서 바로 플레이할 수 있습니다. 이후 같은 브랜치에 수정한 파일을 업로드하면 Pages 배포가 다시 진행됩니다.

참고: [GitHub 공식 문서 — Pages 게시 소스 설정](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Git으로 업로드하기 — 선택 사항

Git이 설치되어 있고 GitHub 인증이 설정되어 있을 때 사용할 수 있습니다. GitHub에서 **비어 있는 새 저장소**를 만든 다음, 이 세 파일이 있는 폴더에서 아래 명령을 실행합니다.

`YOUR-USERNAME`과 `snack-match`는 본인의 계정명과 저장소 이름으로 바꾸세요.

```bash
git init
git add index.html README.md .nojekyll
git commit -m "Add snack matching game"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/snack-match.git
git push -u origin main
```

이미 Git으로 관리 중이거나 원격 저장소에 커밋이 있다면 이 초기화 명령을 그대로 반복하지 말고, 기존 작업 흐름에 맞춰 파일을 추가하세요.

## 기록 저장

진행 상황과 최고 기록은 브라우저 저장소를 사용할 수 있을 때 같은 브라우저에 저장됩니다. 별도의 서버나 계정에 동기화하지 않습니다.

- 브라우저 데이터를 삭제하거나 다른 브라우저·기기·주소에서 열면 기록이 달라질 수 있습니다.
- 시크릿 모드나 저장소 접근 제한이 있는 환경에서는 기록이 유지되지 않을 수 있습니다.
- 파일을 직접 여는 `file://` 환경에서 저장이 제한되면 GitHub Pages 주소로 실행해보세요.

## 문제가 생기면

- **GitHub에서 코드만 보여요:** 저장소의 파일 화면입니다. 게임을 하려면 다운로드한 `index.html`이나 GitHub Pages 주소를 여세요.
- **Pages에서 404가 나와요:** 배포 완료 여부와 브랜치·폴더 설정을 확인하세요. 선택한 폴더에 소문자 `index.html`이 있어야 합니다.
- **수정한 내용이 안 보여요:** 저장소에 커밋이 올라갔는지와 배포 결과를 확인한 뒤 새로고침하세요. Windows에서는 `Ctrl + F5`로 캐시를 무시하고 새로고침할 수 있습니다.
- **이모지가 다르게 보여요:** 운영체제와 브라우저에 따라 간식 그림의 모양이 달라질 수 있습니다.

배포 실패 원인은 저장소의 **Actions** 탭에서도 확인할 수 있습니다.
