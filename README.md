# EXIA 공개 리포트 페이지

Netlify 사용량 한도로 공개 리포트 페이지를 이 저장소의 GitHub Pages로 옮겼습니다.

- 저장소: https://github.com/exiagaram/exiagaram.github.io
- 공개 주소: https://exiagaram.github.io/
- 페이지 경로: `/r/<random 16자 slug>/index.html`
- 검색 비노출: 각 HTML에 `noindex` 메타 태그를 유지합니다. (`robots.txt`도 `Disallow: /`)
- 기존 Netlify 사이트(https://exia-r-od1i1zvxwm.netlify.app)는 지우지 않습니다.

GitHub 계정 `exiagaram`의 user site라서, `main` 브랜치 루트가 자동으로 https://exiagaram.github.io/ 로 배포됩니다. 반영에는 약 1분이 걸립니다.

## 봇 발행 규칙 (필수)

1. 각 봇은 **자기 페이지를 새 `r/<random 16자 slug>/` 폴더에만** 올립니다. slug는 영문 소문자+숫자 16자입니다.
2. **다른 봇의 폴더를 삭제하거나 덮어쓰지 마세요.** 이미 있는 slug는 재사용하지 마세요. 자기 페이지를 수정할 때만 같은 slug의 파일을 업데이트합니다.
3. `netlify.toml`, `_headers`는 올리지 않습니다. 루트에 `.nojekyll`을 유지합니다.
4. 배포는 GitHub 커넥터(`user-GitHub-xai`)의 `push_files`로 `exiagaram/exiagaram.github.io`의 `main` 브랜치에 해당 파일만 푸시합니다. 사이트 전체를 다시 올리지 마세요.
5. 공개 URL은 `https://exiagaram.github.io/r/<slug>/` 입니다. 푸시 후 약 1분 뒤 `curl`로 HTTP 200과 제목을 확인하세요.
6. `gh` CLI 로그인은 쓰지 않습니다. 자격 증명을 다루지 마세요.

## 현재 페이지

| slug | 봇 | 제목 | URL |
|------|----|------|-----|
| elamidda65xo4azj | 마케팅 | EXIA 마케팅 핵심 요약 | https://exiagaram.github.io/r/elamidda65xo4azj/ |
| fridrqqyj568b2u8 | 마케팅 | EXIA 마케팅 전문가 인사이트 | https://exiagaram.github.io/r/fridrqqyj568b2u8/ |
| wd5xwudkndi8xu0k | 브랜딩 | EXIA 브랜딩 핵심 요약 | https://exiagaram.github.io/r/wd5xwudkndi8xu0k/ |
| nxq550hlh70p43j8 | 브랜딩 | EXIA 브랜딩 전문가 인사이트 | https://exiagaram.github.io/r/nxq550hlh70p43j8/ |
| smhcgyw2pyevb179 | 트렌드 | EXIA 트렌드 브리핑 · 11/23(월) | https://exiagaram.github.io/r/smhcgyw2pyevb179/ |

이미지(`.jpg`, `.webp` 등)가 있는 페이지는 HTML과 같은 폴더에 같이 푸시해야 합니다.
