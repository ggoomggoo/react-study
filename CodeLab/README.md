# React를 이용한 웹 서비스 개발하기

* One-day CodeLab with webFrameworks.kr
* http://onoffmix.com/event/72541
* @WePlanet
* @Snippod @이성규
* @2016. 07. 23

---


## 링크

* https://github.com/reactjs/react-tutorial
* https://github.com/shalomeir/snippod-starter-demo-app
* https://github.com/shalomeir/snippod-starter-demo-app-front
* https://github.com/shalomeir/snippod-starter-demo-app-server
* [코드랩 4-1회차 영상 (ReactJS)](http://wepla.net/?p=1573)
* [코드랩 4-2회차 영상 (ReactJS)](#)

## 파일

* [React CodeLab 개발환경 설정 가이드.pdf](https://docs.google.com/document/d/1PPooko0uzUanYZMwKrEUXUWMD3FXCarKhVxGq5_Kip0/edit?pref=2&pli=1)
* [ReactJS_CodeLab_160723.pdf](https://drive.google.com/file/d/0B9ltVFRI_UMiTjdNYzc5UklQTVU/view?pref=2&pli=1)
* [React 참고할만한 자료 모음.docx](https://docs.google.com/document/d/1Rc6ZUQp6kYx6SBPaemo0vP290lBf1nYelErsP2GDgL8/edit?pref=2&pli=1)

## 선수지식

* nodejs
* npm
* ES6
* webpack

## 추가

- pro-react
- [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg?utm_source=chrome-ntp-icon)
- git tag
- babel
- eslint
- Semantic UI

## 진행과정

### 디렉토리 구조 분석
/semantic/src
semantic ui
css
sass
webpack
bundling

/src
/src/client.js
ReactDOM.render( // 시작부분
ReactDOM // 별도로 분리되었음
/src/Root.js // 라우터
/


JSX
프로퍼티는 카멜케이스로 작성

### LAB01a

eslint // airbnb

### LAB01b

propTypes // 컴포넌트의 프로퍼티; 우선 파악하면 좋음;
onClick()
changeColor()
state // 콤포넌트 내부 데이터 // vs prop
this.setState() // thid.*

classnames // lib
state만 관리하면 자동으로 화면을 그려줌

### DATA flow

최상위 컴포넌트(warpper)에서 state 관리하는 것을 추천

### Virtual DOM

setState -> render

### Life Cycle

마운팅
속성 변경
상태 변경
언마운팅

componentWillMount()
componentWillReceiveProps() // setState() 사용

### LAB01c

git checkout -f LAB01c

Card 에 있는속성들을 App으로 이동

ES6 // const

###


### LAB02

app.js - {this.props.children}
radium // style lib
react-helmet // prefix title lib

### LAB02a

react-router // lib
router
App.js
clidren

/src/containers // 개별 react 모듈
/src/layout // 공통 react 모듈

LINK // react-router lib

### LAB02b

/user/:userId 추가

this.props.params
this.location.pathname
this.location.query

const { params } = this.props; // ES6 분할할당

### LAB02c

pushPath()
pushQuery()

react-redux // lib
import { pushPath } from '...'; // this.props
@connect

this.moveToUser = this.moveToUser(this) // this 바인딩

this.refs.* // input ref

### LAB02d

{ key } // = { key: key } // ES6

import $ from 'jquery';


### LAB03

ducks

action
actionCreator
reducer

...state // spread; ES6

export default function ... // import 시 default 만 가져옴

