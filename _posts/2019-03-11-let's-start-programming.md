---
layout: post
title: Let's start programming!
date: 2019-03-11 11:30:30
tags: [수업기록보고서]
comments: true
---

## 프로그래밍의 개념
![programming_banner](https://www.valuecoders.com/blog/wp-content/uploads/2017/09/11-Top-Programming-Trends-To-Look-For-In-20172.jpg)

**프로그래밍**이란 컴퓨터에게 논리적으로 명령을 내리기 위한 과정이다. 그렇다고 해서 아무렇게나 할 수는 없지 않는가. 그렇기에 우리는 먼저 프로그래밍을 하는 방법을 익혀야 한다.

## IDE의 개념과 종류
먼저 프로그래밍은 적당한 환경만 주어진다면 언제 어디서나 할 수 있지만, 대부분은 **IDE(Integrated Development Environment, 통합 개발 환경)** 을 주로 사용할 것이다. 아래는 프로그래밍 수업에서 사용하는 주 IDE를 나열한 표이다.

| 명칭 | 구분 | 기능 |
| :-- | :-- | :-- |
| [Dev-C++](https://sourceforge.net/projects/orwelldevcpp/) | Offline | 완전한 통합개발환경 |
| [IDEONE](https://ideone.com) | Online | 간단한 온라인 개발환경 |

## Dev-C++의 구성과 설정
위 주소로 접속하여 Dev-C++를 설치하자. 그 후 자신이 원하는 장소에 실습 폴더를 생성하고 **도구 - 환경 설정(V) - 파일/디렉토리 - 사용자 기본 디렉토리** 에다가 적용시키자. 그러면 이제 첫 번째 프로젝트를 생성할 준비가 완료된 것이다.

| 단축키 | 기능 |
| :-- | :-- |
| Ctrl + N | 새 파일 생성 |
| Ctrl + W | 현재 파일 종료 |
| Ctrl + S | 현재 파일 저장 |
| Ctrl + E | 현재 라인에서 새 라인 추가 |
| Ctrl + D | 현재 라인부터 라인 삭제 |
| Ctrl + A | 내용 전체 선택 |
| Ctrl + C | 선택된 내용 복사 |
| Ctrl + X | 선택된 내용 잘라내기 |
| Ctrl + V | 선택된 내용 붙여넣기 |

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
