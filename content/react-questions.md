---
title: React 질문
---

https://github.com/hochan222/reactjs-interview-questions-korean#React%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80 를 먼저 훑어보자.

### Why React? 

SyntheticEvent: 브라우저의 기본 이벤트를 감싼 cross-browser wrapper

### React 철학 [링크](https://egas.tistory.com/89)

[We can combine the two by making the React state be the “single source of truth”.](https://reactjs.org/docs/forms.html#controlled-components)

### "key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?

key는 elements 배열을 만들 때 포함시켜야 하는 특수 문자열 속성이다. Keys는 React가 변경, 추가, 제거된 항목을 식별하는 데 도움을 준다.

### refs는 어떻게 사용되는가?

ref는 엘리먼트에 대한 참조를 반환하는 데 사용된다.

경험: 신용카드 만들기에서 자동 focus, contextmenu에서 position 구할때 사용.

### forwardRef는 무엇인가?

특정 컴포넌트에서 ref를 받아 자식에게 전달하는 기능이다.

경험: popup을 만들 때, createPortal을 썼는데 이때 event delegation으로 상위 element에 등록된 이벤트에 대해서, 클릭한 위치의 target을 구하기 위해 사용.

### Virtual DOM이란?

Virtual DOM (VDOM)는 실제 DOM의 인-메모리 표현이다. UI 표현은 메모리에 유지되고 "실제" DOM과 동기화된다. 이는 렌더 함수의 호출과 화면상 elements를 표현하는 사이에 발생하는 단계이다. 이 전체 프로세스는 reconciliation 이라고 한다.


Virtual DOM는 브라우저 API를 기반으로 Javascript 라이브러리로 구현된 개념이다.

### Virtual DOM은 어떻게 작동하나?

Virtual DOM는 세 가지 간단한 단계로 작동한다.

- 기본 데이터가 변경될 때마다, 전체 UI는 Virtual DOM 표현으로 리렌더링 된다.
- 이전 DOM 표현과 새로운 표현 사이의 차이를 계산한다.
- 계산이 완료되면, 실제 DOM은 실제로 변경된 것만 업데이트할 것이다.

### React Fiber란?

Fiber는 React v16에서 새로운 reconciliation(조정된) 엔진 또는 핵심 알고리즘의 재구현이다. React Fiber의 목표는 애니메이션, 레이아웃, 제스처, 작업 일시중지, 중단, 재사용 같은 영역에 대한 적합성을 높이고 다양한 유형의 업데이트에 우선순위를 정하는 것이다.

주요 기능은 `incremental rendering`으로 렌더링 작업을 청크(chunk)로 분할하고 여러 프레임에 걸쳐 펼치는 기능이다.

### Controlled Components, Uncontrolled components [링크](https://egas.tistory.com/88)

### React에서 Lifting State Up란?

여러 컴포넌트가 동일한 변경 데이터를 공유해야 하는 경우 가장 가까운 공통 조상으로 lift the shared state up을 하는 것.

즉, 2개의 자식 컴포넌트가 부모로부터 동일한 데이터를 공유하는 경우, 모든 자식 컴포넌트에서 로컬 상태를 유지하는 대신에 상태를 부모에서 관리하는 것이다.

### React에서 Component란?

React의 Component는 상위 component에서 받은 props 를 input으로 하고 React를 구성하는 가장 작은 단위인 Element 를 output으로 하는 함수이다.

