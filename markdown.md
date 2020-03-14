1.마크다운(.md) 사용법
======================

1.1 헤더(Headers)
-----------------
* 큰제목 : 문서제목

```
This is an H1
=============
```

This is an H1
=============

* 작은제목 : 문서부제목
```
This is an H2
-------------
```

This is an H2
-------------

* 글머리 : #1~6까지만 지원
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
####### This is a H7
```


# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6   
####### This is a H7 (지원하지 않음)

1.2 블럭인용문자(BlockQuote)
----------------------------
블럭인용문자 ```>```를 사용한다.
```
>This is first blockquote
>>This is second blockquote
>>>This is third blockquote
```


>This is first blockquote
>>This is second blockquote
>>>This is third blockquote

blockquote안에서는 다른 마크다운 요소를 포함할 수 있다.

>#### This is H4
>* List   
>```code```

1.3 목록(List)
---------------
* **순서있는 목록(번호)**
순서있는 목록은 숫자와 점을 사용한다.
```
1. 첫번째
2. 두번째
3. 세번째
```

1. 첫번째
2. 두번째
3. 세번째

(순서는 내림차순으로 정의된다.)

* **순서없는 목록(글머리 기호 ```*```,```+```,```-``` 지원)**
```
* 빨강   
  * 노랑
    * 파랑
    
+ 빨강
  + 노랑
    + 파랑

- 빨강
  - 노랑
    - 파랑
```
* 빨강   
  * 노랑
    * 파랑
    
+ 빨강
  + 노랑
    + 파랑

- 빨강
  - 노랑
    - 파랑

혼합 사용도 가능하다.
```
* 빨강
 +주황
  -노랑
   -초록
```
* 빨강
 +주황
  -노랑
   -초록
