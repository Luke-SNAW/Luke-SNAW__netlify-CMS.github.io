# [Articles](./articles)
# [VS code extensions](vs-code-extensions.md)
---
# Dev journal

# 2020/09

## 2020/09/19
### Material-UI
It doesn't work with react form hook.\
To work with that, Custom form control is required.\
Next time, I will use another CSS framework.

Material-UI has issue with next.js
> Warning: Prop `className` did not match. Server: "MuiBox-root MuiBox-root-23" Client: "MuiBox-root MuiBox-root-1"

Maybe these links are useful.
- [Server Rendering](https://material-ui.com/guides/server-rendering/)
- https://github.com/nblthree/nextjs-with-material-ui-and-styled-components/blob/master/.babelrc

## 2020/09/17
### react
setState seems to send rendering signal.\
When list data is updated and bool of toast is setStated, two is rerendered.\
When two data is updated not setStated, nothing changes in DOM.

setState는 refersh 시그널을 주는 듯.\
list update는 데이터만 변경하고 toast 띄우는 bool은 setState 했는데 둘 다 화면에 갱신됨.\
둘 다 데이터 변경했을 때는 화면 변경 없음

## 2020/09/14

### react
Why is datepicker onChange event triggered twice?

## 2020/09/13
### firestore
update timestamp to firestore
### react hook
Hook in hook -> error\
So I extracted hook bind variables into top depth to use its to update in child components.\
If it doens't work, I would try to insert child components into top level parent component.\
If it also doens't work, I would try to use state libary like redux.\
But, first try worked fine.

hook 안에 hook은 error.\
그래서 child에서 useState로 update하기 위해 훅에 쓰이는 변수를 최상단으로 빼냄.\
안되면 child들은 최상단 function 안에 depth 하나 추가해서 넣는걸 시도하고\
그래도 안되면 redux 같은 state library를 쓰려고 했는데 잘되는군.

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
