1.마크다운(.md) 사용법
====================
< 원문 : https://gist.github.com/ihoneymon/652be052a0727ad59601 >   
※개인적인 마크다운 학습용도로 작성한 글입니다.

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
   + 주황
      - 노랑
         - 초록
```
* 빨강
    + 주황
        - 노랑
            - 초록

1.4 코드(Code)
--------------
### 1.4.1 들여쓰기
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.
```
This is a normal paragraph:

   This is a code block.
   This is test code.
   
end code block.
```

This is a normal paragraph:

   This is a code block.
   This is test code.
   
end code block.

-------------------------
> 한 줄을 띄어쓰지 않으면 인식이 제대로 되지 않는다.
```
This is a normal paragraph:
   This is a code block.
   This is test code.
end code block.
```

This is a normal paragraph:
   This is a code block.
   This is test code.
end code block.
