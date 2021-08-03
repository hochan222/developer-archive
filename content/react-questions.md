---
title: React 질문
---

## 목차

- [Why React?](#Why-React?)

### Why React? 

SyntheticEvent: 브라우저의 기본 이벤트를 감싼 cross-browser wrapper

### "key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?

key는 elements 배열을 만들 때 포함시켜야 하는 특수 문자열 속성이다. Keys는 React가 변경, 추가, 제거된 항목을 식별하는 데 도움을 준다.

### refs는 어떻게 사용되는가?

ref는 엘리먼트에 대한 참조를 반환하는 데 사용된다.

경험: 신용카드 만들기에서 자동 focus, contextmenu에서 position 구할때 사용.

### forwardRef는 무엇인가?

특정 컴포넌트에서 ref를 받아 자식에게 전달하는 기능이다.

경험: popup을 만들 때, createPortal을 썼는데 이때 event delegation으로 상위 element에 등록된 이벤트에 대해서, 클릭한 위치의 target을 구하기 위해 사용.

