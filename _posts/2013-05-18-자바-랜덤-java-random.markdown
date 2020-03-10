---
layout: post
title:  "자바 랜덤 java random"
date:   2013-05-18 12:22:00 +0900
categories: dev lagacy
---
`import java.util.Random;`

패키지를 먼저 불러와주고
이후에,
```
Random 랜덤이름 = new Random();
int i = 랜덤이름.nextInt(10) + 1;
```
이는 1~10까지 랜덤한 정수를 생성한다.

+1을 빼면 0~9 까지 이겠지.
