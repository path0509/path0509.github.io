---
layout: post
title:  "ARC(Automatic Reference Counting) 이란 무엇인가?"
date:   2016-06-25 17:33:00 +0900
categories: dev lagacy
---
ARC (Automatic Reference Counting).

자바에 비유하자면, Garbage Collection 과 비슷한 개념.
사용하지 않는 자원을 자동으로 회수한다.

```
한 ViewController 안에 let x = Person() 라는 코드가 있다고 보자.
ViewController가 생성될 때 상수 x는 새롭게 생성된 Person이란 객체를 참조하게 되고, 참조 카운터인 ARC는 1이 된다.
ViewController가 해제될 때 상수 x와 생성된 Person의 연결은 끊어지게 되고, ARC는 0 된다.
즉, 참조하는 곳이 없으므로 더 이상 존재할 필요가 없고 시스템은 Person객체가 점유한 자원을 회수한다.
```

2011년 ARC의 도입에 따라 기존 Garbage Collection과 혼용하여 사용하게 됐다.
2015년 5월부턴 Garbage Collection을 사용한 앱은 심사거절, ARC를 의무적으로 사용하게 됐다.


참고
1. http://imackorea.com/2015/08/스위프트-배우기-swift-strong-reference/
2. http://macnews.tistory.com/3083
