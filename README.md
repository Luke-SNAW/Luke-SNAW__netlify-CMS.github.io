# [VS code extensions](vs-code-extensions.md)
---
# Dev journal

# 2020/09

## 2020/09/12
### Material-UI, tailwindcss
>🌟change css framework to Material-UI Alpha channel v5 from tailwindcss

tailwindcss doesn't has UI components. Even it resets default style like `<button>`. `<button>` is displayed as text.\
It is solely for customizing from start.\

tailwindcss는 프로젝트 완전 처음부터 커스텀 컴포넌트를 만들기 위해 default style도 reset해버리고 셋업에 도움되는 기능들로 구성됨.\
`<button>`이 그냥 텍스트로 나오는거 보고 놀람.

Material은 그냥 github star 수가 가장 많아서 선택 60k.

## 2020/09/11
### flutter
ver. 1.20.1-pre

🌟 Build function is 22 times during **showMaterialBottomSheet**. It's hard to request network in child.\
🌟 Once built during **showBottomSheet**.
### tools
- 🌟 [docz](https://github.com/doczjs/docz) : react document. component documentation ok. logic?
- 🌠 [tailwindcss](https://tailwindcss.com/) : A utility-first CSS framework
- 🌟 [PurgeCSS](https://github.com/FullHuman/purgecss) : It removes unused selectors from your css, resulting in smaller css files.
- ⭐ [react-grid-layout](https://github.com/strml/react-grid-layout) : ![demo](https://camo.githubusercontent.com/8c68a2e6d6e01364247232267a5698ac0d9b63c6/687474703a2f2f692e696d6775722e636f6d2f6f6f314e5436632e676966)

### moment
pretty easy to use. It serves functions which made in previous vue project.\
꽤 편하다. 전에 vue로 작업한 function들을 react로 옮기다가 moment를 써봤는데 다 있는 기능들.

## 2020/09/10
### github page
I read about Jekyll, liquid document to make github page.\
Next.js seemed be better.

## 2020/09/09
### react
🌠 Display data fetched from firestore by using **useState**\
but, array put in setState causes infinite loop\
🌠 **useEffect**'s second parameter solves it.
### github page
🌠 create git page repository

## 2020/09/08
### firestore
Data can't be fetched from firebase.\
🌠 learn about **firebase security rules**.\
⭐ learn **deploy** command of firebase cli.
