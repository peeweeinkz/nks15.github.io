---
layout: post
title: Let's start programming!
subtitle: First class: Concept, IDE, Dev-C++, Hello World, Escape Sequence
date: 2019-03-11 11:30:30
tags: [Class Records Report]
comments: true
---

## The Concept of Programming
![programming_banner](https://www.valuecoders.com/blog/wp-content/uploads/2017/09/11-Top-Programming-Trends-To-Look-For-In-20172.jpg)

**프로그래밍**이란 컴퓨터에게 논리적으로 명령을 내리기 위한 과정이다. 그렇다고 해서 아무렇게나 할 수는 없지 않는가. 그렇기에 우리는 먼저 프로그래밍을 하는 방법을 익혀야 한다.

## The Integrated Development Environment
프로그래밍은 적당한 환경만 주어진다면 언제 어디서나 할 수 있지만, 대부분은 **IDE(Integrated Development Environment, 통합 개발 환경)** 을 주로 사용할 것이다. 아래는 프로그래밍 수업에서 사용하는 주 IDE를 나열한 표이다.

| 명칭 | 구분 | 기능 |
| :-- | :-- | :-- |
| [Dev-C++](https://sourceforge.net/projects/orwelldevcpp/) | Offline | 완전한 통합개발환경 |
| [IDEONE](https://ideone.com) | Online | 간단한 온라인 개발환경 |

## The Management of Dev-C++
![Dev-C++](https://a.fsdn.com/con/app/proj/orwelldevcpp/screenshots/devcpp5200.png/max/max/1)

위 사진이 Dev-C++의 실제 실행 화면이다. 우리도 위 단원의 표에 나열된 주소로 접속하여 Dev-C++를 설치하자. 그 후 자신이 원하는 장소에 실습 폴더를 생성하고 **도구 - 환경 설정(V) - 파일/디렉토리 - 사용자 기본 디렉토리** 에다가 적용시키자. 이제 첫 번째 프로젝트를 생성할 준비가 완료된 것이다.

- 아래의 단축키는 실제 업무 진행 시 유용할 것이니, 암기하자.

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

## Hello, [DSM](https://dsmhs.djsch.kr)!
새 언어에 입문하는 개발자들이 제일 먼저 작성하는 코드는 바로 Hello World!일 것이다. 이때 소스코드 파일을 저장할 경우 파일명의 앞부분에 인덱스(Index) 숫자를 붙이는 것이 좋다.

### 01-HelloDSM.c
{% highlight C linenos %}
#include <stdio.h>

int main() {
	printf("Hello, DSM!\n");
	return 0;
}
{% endhighlight %}

그리고 아래는 해당 코드에 주석으로 각 코드의 역할을 표기한 것이다.

{% highlight C linenos %}
#include <stdio.h> // 전처리문

int main() { // main 함수 시작
    // 코드 작성 시작
    printf("Hello, DSM!\n"); // 문자열 화면표기 // 코드종료
    return 0; // return 구문
    // 코드 작성 종료
}   // 함수 종결
{% endhighlight %}

- 전처리문
   - #이 들어간 문장은 전(前)처리된다.
   - #를 사용하는 이유는 키보드에 할당된 기타 특수문자보다 사용 빈도가 낮았기 때문이다.
- main 함수 시작, 함수 종결
   - {}는 스코프(Scope)라고 하며, 함수의 영역을 표시한다.
   - 스코프 안에서 모든 코드가 시작되고 종결된다.
- 문자열 화면표기문
   - printf() 함수는 문자열을 화면에 표기하는 함수이다.
   - 문자열은 따옴표(")로 묶게 된다.
- 코드종료
   - 모든 명령 코드는 세미콜론(;)으로 종결된다.
- return 구문
   - 인자로 전달된 특정 값을 반환하며, 0은 작업이 성공적으로 종료되었다는 것을 나타낸다.
   - 비슷하게 리눅스/유닉스 OS에서는 'init 0'이 시스템을 재부팅시키는 명령이다.
- \n
   - 개행문자로, 커서를 해당 줄 아래로 이동시킨다.

## The Usage of Escape Sequence
### 02-Alert.c
시작하기 전에 아래 코드를 실행해 보자.
{% highlight C linenos %}
#include <stdio.h>

int main() {
    printf("Alert!!! \a");
    return 0;
}
{% endhighlight %}

{: .box-note}
[경고 소리](https://www.youtube.com/watch?v=MwTcBIqkrsI)가 나는 것을 확인할 수 있을 것이다.

**Question:** 왜 경고 소리가 나는 것일까?

### Code Debugging
**\a**는 이스케이프 시퀀스(Escape Sequence)이다. 이스케이프 시퀀스는 문자열 내에서 사용되었을 때 자기 자신을 나타내지 않고, 특정한 문자나 기능을 재현하게 된다. 이스케이프 시퀀스의 종류는 다음과 같다:

| 이스케이프 시퀀스 | 의미 | 기능 |
| :-- | :-- | :-- |
| \a | Alert | 경고음 재생 |
| \b | Backspace | 백스페이스 |
| \n | New line | 개행 |
| \r | Carriage Return | 전문(前文) 이동  |
| \t | Horizontal Tab | 수평 탭 |
| \v | Vertical Tab | 수직 탭 |
| \\ | Backslash | \ |
| \' | Apostrophe | ' |
| \" | Double Apostrophe | " |
| \? | Question mark | ?  |

