## CRA 프로젝트 github page로 배포하기

### CRA 프로젝트 github 원격 저장소에 올리고 로컬 저장소와 연결하기
1. github repository 생성. README.md는 생성하지 않음
2. local과 연결할 github 주소만 복사하였음
3. 디렉토리에서 npx create-react-app [프로젝트 이름]으로 프로젝트 생성
4. git branch 확인

### Github page 배포하기
1.gh-pages 패키지 설치 

    npm install gh-pages --save-dev



2. package.js 에 “homepage” 주소 추가

    "homepage": "http://holystorySeo.github.io/react-github-pages"



3. script에 predeploy, deploy 추가

    "scripts": {
      //...
      "predeploy": "npm run build",
      "deploy": "gh-pages -d build"
    }
