---
title: HTML 질문
---

## 목차

- [`DOCTYPE`은 무엇을 하나요?](#doctype은-무엇을-하나요)

### `DOCTYPE`은 무엇을 하나요?

[링크](https://egas.tistory.com/86)

`DOCTYPE`은 `document type`의 약어이다. doctype의 유일한 목적은 브라우저가 문서를 렌더링할 때, `quirks mode`로 바뀌지 않도록 하는 것이 유일한 목적이다.

또한, HTML5에서 doctype의 유일한 목적은 `full standards mode`를 활성화하는것이다.

- 세부 설명

옛날에는 웹 페이지가 `Netscape Navigator`, `Microsoft Internet Explorer`로 두 가지 버전이 있었다. W3C에서 웹 표준이 만들어졌을 때, 기존 웹 브라우저와의 호환이 안되어서 바로 사용할 수가 없었다. 따라서, 브라우저는 새로운 표준 준수 사이트를 이전 레거시 사이트와 다르게 처리하기 위해 두 가지 모드를 도입했다. 

현재는 `quirks mode`, `almost standards mode`, and `full standards mode`로 3가지 모드가 존재한다.

`<!DOCTYPE html>`은 HTML5에서 권장하는 방식이다. 오늘날의 모든 기존 브라우저는 `DOCTYPE`에 대해 전체 표준 모드를 ​​사용한다. (Internet Explorer 6 버전도 포함) `DOCTYPE` 이전에 글자가 존재하면 `quirks mode`를 발생시킨다.

이전 버전의 HTML 표준은 `DOCTYPE`에 추가적인 의미를 부여했지만 어떤 브라우저도 쿼크 모드와 표준 모드 사이를 전환하는 것 외에 다른 용도로 `DOCTYPE`을 사용하지 않는다.

단, HTTP 헤더의 MIME 유형을 사용하여 페이지를 `XHTML`로 제공하는 경우 표준 모드를 ​​활성화하기 위해 DOCTYPE이 필요하지 않는다.