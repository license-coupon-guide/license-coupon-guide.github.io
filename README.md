# 엔지니어랩 시크릿코드 — GitHub Pages 업로드 안내

## 사이트 정보
- 네이버에 표시되도록 요청한 사이트명: **엔지니어랩 시크릿코드** (검색엔진 자동 선택이므로 보장되지 않음)
- 홈페이지: https://license-coupon-guide.github.io/
- Organization: `license-coupon-guide`
- Repository: `license-coupon-guide.github.io`
- Visibility: `Public`
- Branch: `main`
- Folder: `/ (root)`

## 첫 배포 순서 (초보자용)
1. GitHub에 로그인한 뒤 `license-coupon-guide` Organization의 사용 가능 여부를 확인하고, 없다면 새로 생성합니다. Organization이 이미 존재하지만 소유하지 않았다면 동일 주소를 사용할 수 없으므로 다른 주소를 선택해야 합니다.
2. Organization 내부에서 새 Repository를 만들고 이름을 **`license-coupon-guide.github.io`** 로 입력합니다. 반드시 **Public** 으로 생성합니다.
3. 다운로드한 ZIP을 **내 컴퓨터에서 먼저 압축 해제**합니다.
4. Repository의 **Add file → Upload files** 를 클릭합니다. 압축 해제한 폴더 자체나 ZIP 파일을 올리지 말고, `index.html`, `assets/`, `robots.txt`, `sitemap.xml`, `favicon.png`, `apple-touch-icon.png`, `.nojekyll`, `README.md` 등 압축 해제한 **내부 파일과 폴더를 저장소 최상위(root)**에 업로드합니다. `index.html`이 저장소 맨 위에 보여야 합니다. (일부 운영체제에서 `.nojekyll`이 숨김 처리될 수 있습니다.)
5. 업로드 화면 하단 **Commit changes** 를 눌러 `main` 브랜치에 반영합니다.
6. **Settings → Pages → Build and deployment → Source: Deploy from a branch** 를 선택하고, **Branch: main, Folder: / (root)** 로 선택한 다음 **Save**합니다.
7. 배포 상태가 완료로 표시되면 https://license-coupon-guide.github.io/ 에 접속해 페이지가 나오는지 확인합니다. 처음에는 배포가 지연될 수 있습니다.
8. 페이지 첫 문단 다음의 **긴 랜딩 이미지를 클릭**하면 새 탭에서 아래 엔지니어랩 e7288 파트너 프로모션 페이지가 열리는지 확인합니다. 이미지 어느 부분에서 클릭해도 동일해야 합니다.

## 필수 링크
- 랜딩 이미지 전체 클릭(엔지니어랩 e7288 파트너 프로모션): https://www.engineerlab.co.kr/ee/promotion/2025/partner/index.php?partnerID=e7288
- 본문 별도 타겟 링크: https://engineerlab-guide.netlify.app/secret-code/
- 기존회원 프로모션(상태/조건 변동 가능): https://www.engineerlab.co.kr/ee/promotion/2025/partner/index.php?partnerID=e7288

## 파일 구조
```text
index.html
assets/
  css/style.css
  images/landing.webp       # 원본 936 × 8416 (크롭/리사이즈 없음)
  images/thumbnail.webp     # 별도 제작한 OG 썸네일 1200 × 1200
favicon.png
apple-touch-icon.png
robots.txt
sitemap.xml
.nojekyll
README.md
```

## 수정 / 재업로드
- 문구 수정은 `index.html`을 수정하고 저장소 최상위 같은 경로에 다시 업로드하여 커밋하면 됩니다.
- 디자인 수정은 `assets/css/style.css` 파일을 교체하면 됩니다.
- 이미지 교체는 `assets/images/`의 같은 파일을 업로드한 후 필요 시 `index.html`의 `width`, `height`를 실제 원본 크기에 맞춰 갱신하세요.
- 변경된 화면이 보이지 않으면 브라우저를 새로고침하고 배포 상태를 확인하세요.

## SEO 확인
- 공개 접속: https://license-coupon-guide.github.io/
- robots: https://license-coupon-guide.github.io/robots.txt
- 사이트맵: https://license-coupon-guide.github.io/sitemap.xml
- OG 이미지: https://license-coupon-guide.github.io/assets/images/thumbnail.webp
- 검색 색인은 실제 배포 이후 네이버 서치어드바이저와 Google Search Console에서 소유 확인 후 제출할 수 있으며 노출 순위를 보장하지 않습니다.
- 네이버·구글 소유 확인 메타 태그는 별도 제공되지 않아 포함하지 않았습니다. 값을 발급받으면 `index.html`의 `<head>` 영역에 삽입하세요.

## 확인할 점
- 본 페이지는 **엔지니어랩 공식 홈페이지가 아닌 독립 정보 사이트**입니다.
- 쿠폰 유효기간, 구성 금액, 적용 가능 상품은 추후 변경될 수 있어 실제 발급 쿠폰과 공식 안내를 우선합니다.
- 이 ZIP을 만든 것만으로 Repository가 생성되거나 GitHub Pages 배포가 자동 완료되는 것은 아닙니다.

## 네이버 통합검색 브랜드 영역 점검
- 홈페이지의 HTML `<title>`은 `엔지니어랩 시크릿코드 | ...` 형식입니다.
- `<meta property="og:site_name">`과 `WebSite.name` JSON-LD 및 화면 헤더·푸터의 명칭을 **엔지니어랩 시크릿코드**로 통일했습니다.
- 파비콘은 기존 `/favicon.png` 주소를 유지하면서 `e7`을 나타내는 독립 디자인으로 교체했습니다. 엔지니어랩 공식 로고는 아닙니다.
- 기존 `index.html`과 CSS, favicon 파일을 함께 교체해야 네이버가 일관된 신호를 수집할 수 있습니다.
- 배포 후 `view-source:https://license-coupon-guide.github.io/`에서 변경된 내용을 확인하고, 네이버 서치어드바이저에서 수집 요청 및 색인 상태를 살펴보세요.
- 네이버의 검색 결과 브랜드명은 **자동 분석으로 결정**됩니다. 위 태그를 적용해도 사이트명이 반드시 노출되는 것은 아니며, 재수집·재처리에 시간이 걸릴 수 있습니다.
- 이 페이지는 엔지니어랩 **공식 홈페이지가 아닌 독립 정보 사이트**입니다.
