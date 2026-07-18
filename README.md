# wownplus_site

㈜와우앤플러스 방문판매·다단계·후원방문판매 전문 솔루션(와우넷) 랜딩페이지.

단일 HTML 랜딩페이지이며 GitHub Pages로 배포됩니다.

## 구성

| 파일 | 설명 |
|------|------|
| `index.html` | 랜딩페이지 본문 (단일 파일, CSS·JS 인라인) |
| `.nojekyll` | GitHub Pages의 Jekyll 처리 비활성화 (정적 파일 그대로 서빙) |
| `WOWnPlus_Logo-Kr_투명.png` | 헤더·푸터 로고 이미지 ※ **직접 추가 필요** |

## 배포 방법 (GitHub Pages)

1. GitHub에서 새 저장소 `wownplus_site` 생성
2. 이 폴더의 파일을 저장소에 업로드(또는 push)
   ```bash
   git init
   git add .
   git commit -m "init: 와우앤플러스 랜딩페이지"
   git branch -M main
   git remote add origin https://github.com/<사용자명>/wownplus_site.git
   git push -u origin main
   ```
3. 저장소 **Settings › Pages** 이동
4. **Source**: `Deploy from a branch` → **Branch**: `main` / `/ (root)` 선택 후 저장
5. 1~2분 뒤 `https://<사용자명>.github.io/wownplus_site/` 에서 확인

## 문의폼(EmailJS) 설정

`index.html` 하단 스크립트의 아래 3개 값을 본인 EmailJS 계정 값으로 교체하세요.
(https://dashboard.emailjs.com)

```js
var EMAILJS_PUBLIC_KEY  = "YOUR_PUBLIC_KEY";
var EMAILJS_SERVICE_ID  = "YOUR_SERVICE_ID";
var EMAILJS_TEMPLATE_ID = "YOUR_TEMPLATE_ID";
```

키를 넣지 않아도 페이지는 정상 작동하며, 이 경우 문의 시 이메일 초안(mailto)이 열립니다.

## 로고 이미지

헤더·푸터 로고는 `WOWnPlus_Logo-Kr_투명.png` 파일을 참조합니다.
이 이미지를 `index.html`과 같은 폴더에 추가해야 로고가 표시됩니다.

## 연락처

- TEL. 02.6083.6919 · FAX. 02.6083.6920
- wownplus@wownplus.co.kr
- 서울시 성동구 성수일로 99, 서울숲AK밸리 1413호
