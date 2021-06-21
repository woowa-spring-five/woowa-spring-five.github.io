# 우아한테크코스3기 스프링5 프로그래밍 입문 스터디 팀 블로그

|수리|알리|현구막|PK|조앤|
|:---:|:---:|:---:|:---:|:---:|
|<img src="/assets/images/dwl5.png" alt="dwl5" width="100" height="100">|<img src="/assets/images/jh8579.png" alt="jh8579" width="100" height="100">|<img src="/assets/images/Hyeon9mak.png" alt="Hyeon9mak" width="100" height="100">|<img src="/assets/images/pkeugine.jpeg" alt="pkeugine" width="100" height="100">|<img src="/assets/images/seovalue.jpeg" alt="seovalue" width="100" height="100">|
|[dwl5](https://github.com/dwl5)|[jh8579](https://github.com/jh8579)|[Hyeon9mak](https://github.com/Hyeon9mak)|[pkeugine](https://github.com/pkeugine)|[seovalue](https://github.com/seovalue)|

|춘식|와일더|김김|욘|크로플|
|:---:|:---:|:---:|:---:|:---:|
|<img src="/assets/images/RinSabbit.png" alt="RinSabbit" width="100" height="100">|<img src="/assets/images/lns13301.png" alt="lns13301" width="100" height="100">|<img src="/assets/images/tributetothemoon.jpeg" alt="tributetothemoon" width="100" height="100">|<img src="/assets/images/thisisyoungbin.jpeg" alt="thisisyoungbin" width="100" height="100">|<img src="/assets/images/perenok.png" alt="perenok" width="100" height="100">|
|[RinSabbit](https://github.com/RinSabbit)|[lns13301](https://github.com/lns13301)|[tributetothemoon](https://github.com/tributetothemoon)|[thisisyoungbin](https://github.com/thisisyoungbin)|[perenok](https://github.com/perenok)|

<br>

## 1. 저자(글쓴이) 설정하기
`/_config.yml` 파일에서 `# Authors` 영역 중 자신의 영역 찾아서 입맛대로 수정하기
```
# Authors
authors:
  pk:                                        -- author 구분자
    name: PK                                 -- 사용할 author 이름
    display_name: 피케이                       -- 블로그에 실제 비춰지는 이름
    avatar: 'assets/images/pkeugine.jpeg'    -- 아바타로 사용될 이미지 경로. 각자 깃허브 프로필 이미지를 따서 저장해두었음.
    email: pkeugine@gmail.com                -- 소개 메일 명.
    web: https://github.com/pkeugine         -- 블로그에서 계정을 클릭했을 때 이동할 웹 경로 (블로그, 깃허브 프로필)
    description: "안녕하세요 피케이입니다 :)"      -- 자기소개
```

`name` 설정의 경우 아래와 같이 실제 포스트를 할 때 `author: `란에 기입하게 된다.
```
---
layout: post
title:  "chapter16-pk"
author: PK                                   -- 사용할 author 이름
categories: [ json, Jackson ]
image: assets/images/13.jpg
---

## JSON (Javascript )
* 간단한 형식을 갖는 문자열로 데이터 교환에 주로 사용한다.

## Jackson
* 자바 객체와 JSON 형식 문자열 간 변환을 처리하는 라이브러리
.
.
.
```

<br>

## 2. 포스트 발행하기
포스트 파일은 `/_posts/*.md` 양식을 기본으로 하되, 파일 명은 자유롭게 정한다.  
포스트를 분리하는 기준(단원별, 분량별) 모두 각자 판단에 따른다.  
단, 다른 크루가 이미 사용중인 파일 명은 사용하지 않도록 주의한다.

포스팅 파일 최상단에는 아래 양식이 필수로 포함되어야 한다.

```
---
layout: post                                -- 글이 블로그에 출력될 형태. post로 고정.
title:  "스프링 MVC 프레임워크와 SpringMVC #1"   -- 블로그에 노출되는 제목.
author: dwl5                                -- /_config.yml 에 설정해둔 author name
categories: [ Chapter9, Chapter10 ]         -- 원하는 카테고리 지정.
tags: [spring, mvc]                         -- 원하는 태그 지정.
image: assets/images/16.jpg                 -- 포스트 썸네일로 노출되는 이미지.
---
```

양식을 모두 포함시킨 후 포스트 내용이 시작되면 된다.


```
---
layout: post                                -- 글이 블로그에 출력될 형태. post로 고정.
title:  "스프링 MVC 프레임워크와 SpringMVC #1"   -- 블로그에 노출되는 제목.
author: dwl5                                -- /_config.yml 에 설정해둔 author name
categories: [ Chapter9, Chapter10 ]         -- 원하는 카테고리 지정.
tags: [spring, mvc]                         -- 원하는 태그 지정.
image: assets/images/16.jpg                 -- 포스트 썸네일로 노출되는 이미지.
---

# Spring MVC

- 스프링 MVC 설정 방법만 익혀두면 웹 개발에 필요한 다양한 기능을 구현할 수 있게 된다.
- DisptacherServlet은 초기화 과정에서 contextConfiguration 초기화 파라미터에 지정한 설정 파일을 이용해서 스프링 컨테이너를 초기화 한다.
  - contextConfiguration의 설정 파일이 AnnotationConfigWebApplicationContext이다.
    - annotation기반 스프링 mvc를 사용하겠다는 의미이다.
- 스프링 MVC 프레임워크에서 컨트롤러란
  - 웹 요청을 처리하고 그 결과를 뷰에 전달하는 스프링 빈 객체
  
.
.
.
```
