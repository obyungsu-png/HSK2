# HSK 학습·시험 안내 사이트

## 세션을 시작하면

- `TODO.md`(남은 작업 목록)를 먼저 읽고, 사용자에게 아직 남은 항목을 짧게 상기시켜 주세요.
- 작업을 끝내거나 새로 미룬 일이 생기면 `TODO.md`를 함께 갱신하세요.

## 구조

- 정적 사이트(서버 없음): `index.html`, `app.js`(화면·라우팅·기본 콘텐츠), `styles.css`, `cms.js`(사이트 관리 화면).
- 운영자가 고친 내용은 `content.json`에 저장되고, 업로드 파일은 `uploads/`에 들어갑니다. `content.json`의 목록이 비어 있으면 `app.js`의 `DEFAULT_LISTS`가 쓰입니다.
- 새 목록을 추가할 때는 `app.js`의 `DEFAULT_LISTS`와 `cms.js`의 `LIST_SCHEMAS`를 함께 추가해야 합니다.
- 페이지는 해시 주소로 나뉩니다(`#levels`, `#teachers`, `#homework` 등). 탭 주소는 `app.js`의 `TAB_ROUTES`를 참고하세요.

## 작성 규칙

- 모든 문구는 한국어·영어·중국어 3개 언어입니다. HTML은 `data-en`/`data-zh` 속성을, JS는 `tri(ko,en,zh)`/`tx(...)`를 씁니다.
- 시험 정보(문항 수, 시간, 점수, 링크)는 공식 출처(chinesetest.cn, hskmock.com)에서 확인한 것만 넣고, 확인한 날짜를 주석에 남기세요.
- 문구는 담백하게 쓰세요. 같은 안내 문구를 페이지마다 반복하지 말고, 파스텔 장식 색은 쓰지 않습니다.
