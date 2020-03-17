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

### 1.4.2 코드블럭 코드
코드를 이용한 코드블럭 생성은 다음과 같이 2가지 방식을 사용할 수 있다.

* ```<pre><code>{code}</code></pre>``` 이용방식 (한 줄 전체를 코드로 인식)
* ```<code>{code}</code>``` 이용방식 (한 줄 이내 코드, 문구)
```
<pre>
<code>
public class HowToUseGit {
    public static void main(String[] args) {
        System.out.println("How to use markdown?");
    }
}
</code>
</pre>
```
<pre>
<code>
public class HowToUseGit {
    public static void main(String[] args) {
        System.out.println("How to use markdown?");
    }
}
</code>
</pre>

* <code>```</code> 이용방식

<pre>
<code>
```
public class HowToUseGit {
    public static void main(String[] args) {
        System.out.println("How to use markdown?");
    }
}
```
</code>
</pre>

```
public class HowToUseGit {
    public static void main(String[] args) {
        System.out.println("How to use markdown?");
    }
}
```

1.5 수평선 ```<hr/>```
---------------------
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 페이지 나누기 용도로 많이 사용한다.
```
* * *

***

*****

- - -

----------------------
```
* 적용 결과

* * *

***

*****

- - -

----------------------

1.6 링크(Links)
----------------
### 1.6.1 참조링크
```
[link keyword] [id]

[id]: URL "Optional Title here"
```

* 예시
```
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
```
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

### 1.6.2 외부링크
```
[Title](link)
```
* 예시
```
링크: [Google](https://google.com, "google link")
```
링크: [Google](https://google.com, "google link")

### 1.6.3 자동연결
일반적인 URL 혹은 이메일주소인 경우 적절한형식으로 링크를 형성한다.
* 예시
```
외부링크: <http://example.com/>
이메일링크: <address@example.com>
```

외부링크: <http://example.com/>
이메일링크: <address@example.com>

1.7 강조(Highlight)
-------------------
```
*single asterisk*
_single underscore_
**double asterisk**
__single underscores__
~~cancelline~~
```

* *single asterisk*
* _single underscore_
* **double asterisk**
* __single underscores__
* ~~cancelline~~

>```문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.```   
>문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.

1.8 이미지
----------------
```
![Alt text](/path/to/image.jpg)
![Alt text](/path/to/image.jpg "Optional title")
```
![Alt text](/path/to/image.jpg)
![Alt text](/path/to/image.jpg "Optional title")
