# 철학맨 김선중의 철학 노래방

모바일 중심으로 만든 정적 웹사이트입니다.

## 구성

- 첫 화면: 제목 + 3열 릴스 카드 그리드
- 카드 선택: 철학 노래 상세 화면
- 상세 화면: 릴스 썸네일 → 인스타그램 링크, 제목, 가사
- 모바일 우선 반응형
- 별도의 서버/DB 없이 바로 실행 가능

## 실제 릴스 이미지와 링크 넣기

`app.js`의 `songs` 배열에서 각 항목을 수정하면 됩니다.

```js
{
  id: "song-01",
  title: "노래 제목",
  artist: "아티스트",
  thumbImage: "assets/my-reel.jpg",
  instagramUrl: "https://www.instagram.com/reel/...",
  lyrics: `가사`
}
```

현재 샘플 버전은 `thumbLabel`을 이용한 디자인 플레이스홀더를 사용합니다.
실제 이미지를 적용할 경우 `thumbImage`를 추가하고 CSS/JS에서 background-image 또는 `<img>`로 연결하면 됩니다.

## 실행

`index.html`을 브라우저에서 열어도 기본 기능을 확인할 수 있습니다.

배포할 때는 GitHub Pages, Netlify, Vercel 등 정적 호스팅에 그대로 올릴 수 있습니다.
