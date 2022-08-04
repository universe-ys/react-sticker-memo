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
