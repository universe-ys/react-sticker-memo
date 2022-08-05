# react-sticker-memo

# Draggable 컴포넌트 개발 & npm 배포

`npx create-react-app draggable`

`npm i underscore`

`npm i -D @babel/cli @babel/preset-react`

```json
// package.json
...
  "scripts": {
    ...
    "publish": "rm -rf dist && mkdir dist && babel src/lib -d dist --copy-files"
  },
  "babel": {
    "presets": ["@babel/preset-react"]
  },
...
```

`npm run publish`

```json
// package.json
{
  "name": "@seulyiyoo/draggable",
  "version": "1.0.0",
  "module": "dist/Draggable.js",
  "main": "dist/Draggable.js",
  ...
}
```

```
# .gitignore

/public
/src
```

`npm login`

`npm publish --access public`

---

# 스티커메모

## 개발환경설정

`npx create-react-app sticker-memo`

`npm i @seulyiyoo/draggable` npm package 사용

`npm i @mui/icons-material @mui/material @emotion/react @emotion/styled` 아이콘 사용

`npm i mobx mobx-react` store 사용

`npm i node-sass` sass 사용

`npm i underscore` throttle / debounce 사용

`npm i uuid` 유니크 id 사용

---
## 프로젝트 시작

### 메모 UI 개발(HTML, SCSS)

### draggable 컴포넌트 적용

### mobx 설정 및 메모 생성

makeObservable / observable / action

### 메모 내용 수정 update

MobX Developer Tools 확장프로그램설치

debounce 로 0.5초마다 갱신

### 메모 크기 변경 update

resizeObserver

useLayoutEffect

contentRect

### 메모 위치 변경 update

### 메모 삭제

### localStorage 연동

autorun
