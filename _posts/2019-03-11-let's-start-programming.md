---
layout: post
title: Let's start programming!
date: 2019-03-11 11:30:30
tags: [수업기록보고서]
comments: true
---

## 프로그래밍의 개념
**프로그래밍**이란 컴퓨터에게 논리적으로 명령을 내리기 위한 과정이다. 그렇다고 해서 아무렇게나 할 수는 없지 않는가. 그렇기에 우리는 먼저 프로그래밍을 하는 방법을 익혀야 한다. 먼저 프로그래밍은 적당한 환경만 주어진다면 언제 어디서나 할 수 있지만, 주로 **IDE(Integrated Development Environment, 통합 개발 환경)**을 사용할 것이다.



You can write regular [markdown](http://markdowntutorial.com/) here and Jekyll will automatically convert it to a nice webpage.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](http://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/headings/tables/etc.

**Here is some bold text**

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


How about a yummy crepe?

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

Here's a code chunk:

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
