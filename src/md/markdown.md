# 마크다운 문법

## 마크다운이란?
2004년 존그루버에 의해 만들어진 **텍스트 기반의 마크업언어**  
문서의 구조를 쉽게 작성하고, 이를 HTML로 변환할 수 있게 해준다.
가독성이 뛰어나며, 서식 적용이 직관적이다.  
주로 README 파일, 블로그 포스트, 문서 작성 등에 사용된다.
<br><br>

## 마크다운의 장/단점

### 장점

1. 간결하다.
2. 별도의 도구없이 작성가능하다.
3. 다양한 형태로 변환이 가능하다.
4. 텍스트(Text)로 저장되기 때문에 용량이 적어 보관이 용이하다.
5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
6. 지원하는 프로그램과 플랫폼이 다양하다.

### 단점

1. 표준이 없다. (도구에 따라서 변환방식이나 생성물이 다르다.)
2. 모든 HTML 마크업을 대신하지 못한다.  
<br>

## 마크다운 문법 정리
### 1. Header

>\# H1: 
># H1

>\## H2:
>## H2

>\### H3:
>### H3

>\#### H4:
>#### H4

<br>

### 2. 목록

순서있는 목록
>```
>1. 첫번째
>2. 두번째
>```
>결과:
>  1. 첫번째
>  2. 두번째

<br>

순서없는 목록: *, +, - 사용
>```
>- 순서
>  - 없는
>    - 목록
>    * 혼합 사용 가능
>    + 혼합 사용 가능
>```
>결과:
>  - 순서
>    - 없는
>      - 목록
>      * 혼합 사용 가능
>      - 혼합 사용 가능

<br>

### 3. 코드블럭
>````
>```markdown(언어지정가능)
>{code block}
>```
>````
>결과:
>```markdown
>{code block}
>```

>```<pre><code>{code}</code></pre>```  
>결과:
><pre><code>{code block}</code></pre>
<br>

### 4. 수평선
>`<hr/>`
><hr/>
><br>  

<br>

### 5. 링크
>참조링크  
>`[link keyword][id]`  
>`[id]: URL "Optional Title here"`  
><pre><code>[Google][googlelink]
>
>[googlelink]: https://google.com "Go google"</code></pre>  
>결과:  
>[Google][googlelink]
>
>[googlelink]: https://google.com "Go google"

>외부링크  
>`[Title](link)`  
><pre><code>[Google](https://google.com, "google")</pre></code>  
>결과:  
>[Google](https://google.com, "google")

>자동연결  
><code>`<http://google.com`>  
>`<emailaddress@gmail.com>`</code>  
>결과:  
><http://google.com>  
><emailaddress@gmail.com>

<br>

### 6. 강조
>```
>*single asterisks* (기울임)
>_single underscores_ (기울임)
>**double asterisks** (굵은글씨)
>__double underscores__ (굵은글씨)
>~~cancelline~~ (취소선)
>```
>
>결과:  
>*single asterisks*  
>_single underscores_  
>**double asterisks**  
>__double underscores__  
>~~cancelline~~

<br>

### 7. 이미지
>`<img width="" height=""></img>`  
>속성: `title`, <code>alt</code>

<br>

### 8. 기타 
>`` `{코드}` ``, `<code>{코드}</code>` : 인라인  
>` ```{코드}``` `, `<pre><code>{코드}</code></pre>` : 코드블록

>\> : 인용문  
>---, ***, ___ : 수평선  
>|, - : 테이블
