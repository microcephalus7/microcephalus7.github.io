---
title: 'TypeGoose 간단 정리'
date: 2021-07-04
categories: BackEnd MongoDB Mongoose TypeGoose
---

# TypeGoose

    TypeScript 의 class 를 사용한 Mongoose model 정의

TypeScript 의 class 를 사용한 Mongoose model 정의

wrapper 로써 쉽게 Mongoose model 을 작성하게 해줌

Mongoose + TypeScript 시 Schema, interface 두가지 다 작성하던 것을 간소화 시켜줌

- 데코레이터

  동기화 문제를 해결하기 위해 사용됨

  - Property

    @prop : Model 이나 Document 의 value 정의 시 사용

    @arrayProp, @mapProp : Deprecated 됨. 사용 지양

  - Class

    @modelOptions : Schema 옵션. Mongoose 연결 위해 쓰임

    @index : prop 에 정의되지 않은 index 위해 쓰임

    @plugin : 플러그인 추가 시 쓰임. prop 타입 수정할 수 없음

    @queryMethod : 쿼리 메소드 추가 시 쓰임

  - Hooks

    @pre : 특정 함수 실행 전 실행

    @post : 특정 함수 실행 완료 뒤 실행
