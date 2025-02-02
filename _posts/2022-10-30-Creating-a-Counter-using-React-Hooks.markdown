---
layout : post
title : Creating a Counter using React Hooks
subtitle : Let's make a counter using React Hook
categories : React
tags : [React, Hook, Counter]
---

## 01. React Hook
Hook은 함수 컴포넌트에서 React state와 생명주기 기능(lifecycle features)을 “연동(hook into)“할 수 있게 해주는 함수이다.<br>
Hook은 class 안에서는 동작하지 않는다. 대신 class 없이 React를 사용할 수 있게 해준다.<br>
- Hook의 사용 규칙
  1. 최상위(at the top level)에서만 Hook을 호출해야 한다. 반복문, 조건문, 중첩된 함수 내에서 Hook을 실행할 수 없다.
  2. 직접 작성한 custom Hook 내 or React 함수 컴포넌트 내에서만 Hook을 호출해야 한다.

## 02. React Hook을 이용한 Counter 만들기

{% include codepen.html hash = "MWXapLv" title = "React hook Counter" %}

## 03. Reference
- [Hook 개요](https://ko.reactjs.org/docs/hooks-overview.html)
- [Basic React Hooks Example - Josh Collinsworth](https://codepen.io/collinsworth/pen/eXxRZb)