# zianplay/policies

(주)지안플랫폼 모바일 앱의 **개인정보처리방침 / 이용약관** 호스팅.
GitHub Pages로 정적 서빙한다. 스토어 심사·앱 내 링크가 이 URL을 가리킨다.

## 공개 URL

- 허브: `https://zianplay.github.io/policies/`
- 도란책방 개인정보처리방침: `https://zianplay.github.io/policies/doranbookstore/privacy.html`
- 도란책방 이용약관: `https://zianplay.github.io/policies/doranbookstore/terms.html`

## 구조

```
policies/
├─ index.html              앱 목록 허브
├─ assets/doc.css          공유 스타일 (디자인 변경은 여기서만)
├─ doranbookstore/
│  ├─ privacy.html
│  └─ terms.html
└─ .nojekyll               순수 정적 파일로 서빙 (Jekyll 처리 안 함)
```

## 새 앱 추가

1. `<앱이름>/` 폴더 생성, `privacy.html` · `terms.html` 작성
   (기존 `doranbookstore/*.html`을 복사해 `<link href="../assets/doc.css">` 유지)
2. `index.html`에 `app-card` 블록 하나 추가
3. 커밋 → 푸시하면 GitHub Pages가 자동 반영

## 문서 개정

- 각 페이지의 시행일(`.effective`)과 본문을 수정하고 커밋
- 앱 코드 저장소의 `docs/*.md`가 원본 참고본 — 함께 갱신
- 중요한 변경은 시행일 최소 7일 전(약관은 불리·중대 변경 시 30일 전) 앱 내 공지

## GitHub Pages 설정

Settings → Pages → Build and deployment → Source: **Deploy from a branch** →
Branch: `main` / `/ (root)`
