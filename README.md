# vite를 이용한 포트폴리오 사이트 만들기

## vite를 사용하는 이유

[vite](https://ko.vitejs.dev/guide/)
웹 애플리케이션을 더 빠르게 개발하고 더 빠르게 빌드하는 것을 목표로 합니다.

## Vite의 주요 특징

1. 빠른 개발 서버: Vite는 개발 서버를 통해 코드를 실시간으로 빠르게 빌드하고 제공합니다. 이로써 개발자는 빠른 리로드 및 개발 환경에서의 빠른 피드백을 얻을 수 있습니다.
2. 빠른 빌드: 프로덕션 빌드 시 Vite는 최적화된 빌드 프로세스를 사용하여 작은 번들 크기와 빠른 로딩 속도를 제공합니다.
3. ES 모듈 기반: Vite는 기본적으로 ES 모듈을 사용하며, 개발 시에 각 모듈을 개별적으로 불러오므로 불필요한 코드를 로드하지 않아 최적화가 용이합니다.
4. Vue.js 지원: Vite는 Vue.js를 위한 개발 환경을 최적화하였으며, Vue.js 프로젝트에서 사용하기에 이상적입니다.
5. 다양한 플러그인 및 확장성: Vite는 다양한 플러그인을 지원하며, 사용자 정의 설정을 통해 프로젝트에 맞는 개발 환경을 구축할 수 있습니다.

## 설치

`npm run dev` 실행하기
`npm i @studio-freight/lenis` lenis 설치

## 구현 기능

- 구글 폰트 적용
- smooth 효과 적용 : [Link](https://lenis.studiofreight.com/)
- 자바스크립트 메뉴 클릭 이동 효과 적용
- GSAP를 이용한 가로 효과
- JavaScript 모듈 기능 적용
- 웹표준 준수를 위한 스킵 메뉴 및 aria, role 적용
- Vite 빌드 작업
- Netilfy 배포 작업

## 트러블 슈팅

<details>
<summary>git 업로드 버그</summary>

<!-- summary 아래 한칸 공백 두어야함 -->

## git 업로드 권한 버그(해결) :

# 권한으로 인한 업로드 버그 해결

윈도우 자격증명 > git 아이디 변경
`git remote set-url origin https://github.com@audgns722/vite-project2023.git` > `git push -u origin master`
깃헙 패스워드 입력을 하라는 창이 나오고 입력을 하시면 본인의 깃주소에 소스코드가 올라갑니다.
인증이 끝난 후부터는 git push만 하면 기존의 세팅한 주소로 바로 푸쉬가 됩니다.

</details>

<details>
<summary>Whitespace 에러</summary>

<!-- summary 아래 한칸 공백 두어야함 -->

## Whitespace 에러(해결) :

# push 중 warning

[해결!](https://velog.io/@wnguswn7/Git-Bash-warning-in-the-working-copy-of-.gitignore-LF-will-be-replaced-by-CRLF-the-next-time-Git-touches-it)  
Git의 core.autocrlf 라는 기능을 켜서 이를 자동 변환 해주도록 하면 된다.

- `git config --global core.autocrlf true` // 시스템 전체에 적용
- `git config core.autocrlf true` // 해당 프로젝트에만 적용
</details>
