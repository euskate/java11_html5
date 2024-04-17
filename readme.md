# HTML 란?

- HTML(Hyper Text Markup Language) 는 웹 환경(Hyper)에서 그 내용을 볼 수 있도록 한 마크업 언어로서 각 요소를 태그(tag) 라고 하는데, 마크업은 이 태그를 여는 부분과 닫는 부분의 사이에 표시할 내용을 마크업한다고 말합니다.
- 여기서 웹 페이지(web page)는 월드 와이드 웹 상에 있는 개개의 HTML로 작성된 문서를 가리킵니다. 
- .gif, jpg, .ai, .pdf, .doc, .hwp 이와 같은 확장자 포맷(형식)이 있듯이 HTML 은 .htm, .html 확장자 포맷을 가지고 있습니다. 
- html 문서는 단순히 텍스트 파일에 불과하고 웹 브라우저가 해석을 해서 구조를 통해 화면에 렌더링 해주게 되고 사용자는 View 라고 하는 스크린(브라우저 화면)을 통해 접하게 되는 것입니다.
- 현재는 웹 문서의 표준을 HTML5 로 규정하고 있습니다.


## 1. HTML의 기본 문서 구조

- HTML은 머리(head)와 몸(body)로 이루어져있다고 생각하면 편합니다.
- head는 HTML의 전반적인 특성을 설정하는 곳 입니다.
- body는 화면에 출력될 내용들을 마크업하는 곳 입니다.
- 모든 태그는 <여는태그> </닫는태그> 가 같습니다. 다만, 일부 태그인 link, meta, input, img 태그 등은 여는태그 부분만 존재하는 몇 가지 예외되는 태그가 있습니다.
- 태그에는 기본(필수) 속성과 추가 속성 등을 지정하게 됩니다.
- 모든 태그는 정식 명칭은 요소(Element)라고 합니다.

```comment
<!DOCTYPE html>
<html>
    <head>
        <!-- 태그 내에서의 각주 -->
        <title></title>
        <meta />
        <link rel="" href="" />
        <style>
        /* 스타일 태그 내부의 각주 */
        </style>
        <script>
        //스크립트 태그 내부의 한 줄 각주
        /*
        스크립트 태그 내부의
        여러 줄 각주
        */
        </script>
    </head>
    <body>
        <a href=""></a><!-- a 태그의 기본 속성은 href입니다. -->
        <img src="" alt=""><!-- img 태그의 기본 속성은 src와 alt 속성입니다. -->
        <!-- input 요소의 기본 속성은 type 속성이며, name, id, class는 추가 속성입니다. -->
        <input type="text" name="" id="" class="">
    </body>
</html>
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>기본 웹 문서</title>
    <!-- 이 곳의 문서의 특성이나 설정, 화면 출력전에 해야 할 일들을 마크업합니다. -->
    <!-- 이 곳에는 link, title, meta, style, script 태그 등을 필요에 따라 마크업할 수 있습니다. -->
</head>
<body>
    <!-- 이 곳의 화면에 출력될 내용들을 마크업합니다. -->
</body>
</html>
```

<br><hr><br>

## 2. HEAD 내부 요소

| 용도명 | 태그명 | 설명 | 사용예 |
|---------------|--------| ----------------------------------------------------|-------------------------------------------------------------|
| 페이지 제목 | title | 현재 웹페이지의 탭에 나타나는 제목을 설정합니다. | &lt;title&gt;가산동에 오신 것을 환영합니다.&lt;/title&gt; |
| 뷰포트 설정 | meta | 현재 웹페이지의 화면출력에 대한 설정을 합니다. | &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt; |
| SEO 페이지 제목 | meta | 현재 웹페이지가 검색엔진에 노출되었을 때의 제목부를 나타냅니다. | &lt;meta name="subject" content="가산동 소개(Gasandong Intro)" /&gt; |
| SEO 페이지 설명 | meta | 현재 웹페이지가 검색엔진에 노출되었을 때의 설명부를 나타냅니다. | &lt;meta name="description" content="가산동, 패션, 아웃렛, IT빌딩, 디지털산업단지, 가산동 맛집" /&gt; |
| SEO 페이지 검색어 | meta | 현재 웹페이지가 검색엔진에 잘 노출될 수 있는 검색 단어를 설정합니다. | &lt;meta name="keywords" content="가산동, 패션, 아웃렛, IT빌딩, 디지털산업단지, 가산동 맛집" /&gt; |
| 오픈그래프 타입 | meta | 현재 페이지의 URL을 다른 애플리케이션이나 SNS 등에 보낼 때 표시될 애플리케이션 정보에서 애플리케이션의 타입을 설정합니다. | &lt;meta property="og:type" content="website" /&gt; |
| 오픈그래프 제목 | meta | 현재 페이지의 URL을 다른 애플리케이션이나 SNS 등에 보낼 때 표시될 애플리케이션 제목부를 설정합니다. | &lt;meta property="og:title" content="gasandong" /&gt; |
| 오픈그래프 설명 | meta | 현재 페이지의 URL을 다른 애플리케이션이나 SNS 등에 보낼 때 표시될 애플리케이션 설명부를 설정합니다. | &lt;meta property="og:description" content="가산동, 패션, 아웃렛, IT빌딩, 디지털산업단지, 가산동 맛집" /&gt; |
| 오픈그래프 이미지 | meta | 현재 페이지의 URL을 다른 애플리케이션이나 SNS 등에 보낼 때 표시될 애플리케이션 썸네일을 설정합니다. | &lt;meta property="og:image" content="./images/site.png" /&gt; |
| App 아이콘 설정 | link | 웹 애플리케이션이 설치되었을 때 나타나는 아이콘을 지정합니다. | &lt;link rel="icon" href="./images/favicon.png" /&gt; |
| 바로가기 아이콘 설정 | link | 웹 애플리케이션이 실행되었을 때 나타나는 페이지 탭에 나타나는 아이콘을 지정합니다. | &lt;link rel="shortcut icon" href="./images/favicon.png" /&gt; |
| 외부 스타일 가져오기 | link | 외부 스타일인 .css 파일을 가져올 때 지정합니다. | &lt;link rel="stylesheet" href="./css/bootstrap.min.css" /&gt; |
| CDN 방식으로 스타일 불러오기 | link | 외부 사이트에서 해당 스타일 파일을 다운로드 받지 않고, 직접 URI를 연결하여 외부 스타일을 로딩합니다. | &lt;link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.0/css/all.css" /&gt; |
| 내부 스타일 지정 | style | 현재 문서에 있는 태그나 요소에 대한 CSS 스타일을 지정합니다. | &lt;style&gt; * { margin:0; padding; } &lt;/style&gt;
| 내부 스크립트 | script | 본문인 body 요소의 내용을 로딩하기 전에 처리해야 하는 부분을 기술합니다. | &lt;script&gt; alert("해당 내용 로딩") &lt;/script&gt; |
| 외부 스크립트 | script | 본문의 body 요소의 내용을 로딩하기 전에 외부 스크립트 파일을 로딩하여 처리합니다. | &lt;script src="./js/bootstrap.min.js" &gt;&lt;/script&gt; |


<br><hr><br>

## 3. 제목 및 문단/글자 요소

- 제목은 h1~h6 범위 안에서 아래의 예시와 같이 입력합니다.
- h1 요소의 글자 크기가 가장 크며, h6 요소의 글자 크기가 가장 작습니다.
- p 요소는 문단을 나타내는 요소입니다.
- span, strong, em, ins 등은 
- span 요소는 한 단어나 한 글자 이상의 내용을 분리할 경우 활용됩니다.
- strong 요소는 한 단어나 한 글자 이상의 내용을 굵게 표시하여 강조할 경우 활용됩니다.
- em 요소는 한 단어나 한 글자 이상의 내용을 기울임꼴로 표시하여 강조할 경우 활용됩니다.
- ins 요소는 한 단어나 한 글자 이상의 내용을 밑줄을 표시하여 강조할 경우 활용됩니다.
- h1~h6 요소와 p 요소는 블록 요소이므로 크기(폭/높이)와 모든 바깥여백과 안여백을 적용할 수 있습니다.
- span, strong, em, ins 등은 인라인 요소이므로 크기(폭/높이) 지정이 되지 않으며, 위/아래 바깥여백과 위/아래 안여백을 적용할 수 없습니다.
- br 요소는 한 문단 내에서 줄바꿈할 경우 사용하되, 가급적 자동 줄바꿈 구간에서는 사용하지 않는 것이 좋습니다.
- ``` &nbsp; ``` 와 같은 문자는 띄워쓰기 문자이며, 웹 문서에서는 여러 칸을 띄워도 한 칸 밖에 띄워지지 않으로므로 여러 칸을 띄울 경우 ``` &nbsp; ``` 를 띄울 칸 수 만큼 넣으시면 됩니다.

<br>

### 3-1. 기본 문법

- h1~h6, p 요소는 서로 겹쳐 쓸 수 없으며, 본인 요소도 겹쳐 쓸 수 없습니다.
- h1~h2 요소는 대제목인 페이지 제목이나 큰 영역의 제목에 사용됩니다.
- h3~h4 요소는 중제목인 항목제목 등에 사용됩니다.
- h5-h6 요소는 소제목인 설

```comment
<h1>제목</h1>
<p>문단 내용 <span>단어</span> <strong>굵게</strong> <em>이태릭</em> <ins>밑줄</ins> </p>
```

<br>

### 3-2. 기본 예시

```html
<h1>h1입니다.</h1>
<h2>h2입니다.</h2>
<h3>h3입니다.</h3>
<h4>h4입니다.</h4>
<h5>h5입니다.</h5>
<h6>h6입니다.</h6>
<p>
    <span>우리 나라</span> <br><strong>대한&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;민국</strong>
    <em>살기 좋은</em> 나라 <ins>대한민국</ins>
</p>
```

<br><hr><br>

## 4. 목록 요소

- ul(Unordered List)은 비순서형 목록으로 내부 안에 자식 요소는 반드시 li 태그가 되어야 합니다.
- ol(Ordered List)은 순서형 목록으로 내부 안에 자식 요소는 반드시 li 태그가 되어야 합니다.
- dl(Definition List)은 사전형태의 정의형 목록으로 내부 안에 자식 요소는 dt(그룹제목)과 dd(그룹항목) 이어야 합니다.
- li 요소는 부모 요소로 반드시 ul 또는 ol이어야 합니다.
- ul, ol, dl 요소는 서로 중첩 사용이 가능하여 다단계 중첩 메뉴인 2단 메뉴, 3단 메뉴 등을 구성할 수 있습니다.
- ul이나 ol 요소는 중첩할 경우 1단계와 2단계의 목록기호나 타입이 서로 달라집니다.
- ul, ol, dl, li, dt, dd 요소는 블록요소로서 크기(폭/높이) 지정과 모든 바깥여백과 안여백을 지정할 수 있습니다.

<br>

### 4-1. UL 또는 OL 의 목록 기호의 Type

- ul 요소나 ol 요소는 li 요소 앞에 표시할 타입을 type 속성을 활용하여 지정할 수 있습니다.
- ol 요소는 start 속성을 이용해 시작값을 지정할 수 있습니다.
- ol 요소 내에서 중간에 숫자를 건너뛸 경우 li 요소에 value 값을 지정하여 중간에 숫자를 건너뛸 수 있습니다.

| type | 설명 |
|------|----------------------------------------------------------|
| circle | 안이 채워진 원이 목록기호로 설정됩니다. |
| disc | 안이 채워진 원이 목록기호로 설정됩니다. |
| square | 안이 채워진 정사각형 목록기호로 설정됩니다. |
| 1 | 아라비아 숫자로 1, 2, 3... 의 순으로 목록숫자로 설정됩니다. |
| a | 영문 소문자로 a, b, c... 의 순으로 목록숫자로 설정됩니다. |
| A | 영문 대문자로 A, B, C... 의 순으로 목록숫자로 설정됩니다. |
| i | 로마자 소문자로 i, ii, iii... 의 순으로 목록숫자로 설정됩니다. |
| I | 로마자 대문자로 I, II, III... 의 순으로 목록숫자로 설정됩니다. |

<br>

### 4-2. 목록 요소 기본 문법

```comment
<ul>
    <li>비순서목록1</li>
    <li>비순서목록2</li>
    ....
</ul>
<ol>
    <li>순서목록1</li>
    <li>순서목록2</li>
    ....
</ol>
<dl>
    <dt>그룹제목</dt>
    <dd>항목1</dd>
    <dd>항목2</dd>
    ....
</dl>            
```

<br>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>목록 연습</title>
</head>
<body>
    <h2>목록 태그</h2>
    <hr>
    <h3>순서있는 목록 : ol</h3>
    <p>반드시 자식 요소가 li가 되어야 한다.</p>
    <ol>
        <li>목록1</li>
        <li>목록2</li>
        <li>목록3</li>
        <li>목록4</li>
        <li>목록5</li>
    </ol>
    <ol type="I">
        <li>로마자</li>
        <li>대문자</li>
        <li>목차</li>
        <li>대한민국</li>
        <li>우리나라</li>
    </ol>
    <hr>
    <h3>순서 없는 목록 : ul</h3>
    <p>반드시 자식 요소는 li 요소이어야 한다.</p>
    <ul>
        <li>한식 뷔페
            <ul>
                <li>제육볶음
                    <ul>
                        <li>당근 제육볶음</li>
                        <li>감자 제육볶음</li>
                    </ul>
                </li>
                <li>김밥</li>
            </ul>
        </li>
        <li>떡볶이
            <ul>
                <li>밀 떡볶이</li>
                <li>쌀 떡볶이</li>
                <li>치즈 떡볶이</li>
            </ul>
        </li>
        <li>불고기
            <ul>
                <li>간장 파 불고기</li>
                <li>고추장 불고기</li>
            </ul>
        </li>
        <li>돈까스
            <ul>
                <li>등심 돈까스</li>
                <li>치즈 돈까스</li>
            </ul>
        </li>
    </ul>
    <ul type="square">
        <li>김기태</li>
        <li>강감찬</li>
        <li>이순신</li>
    </ul>    
    <hr>
    <h3>정의형 목록 : dl</h3>
    <p>자식 요소로 카테고리 그룹명에는 dt 요소를, 그룹 요소들은 dd 요소를 사용해야 한다.</p>
    <dl>
        <dt>Company</dt>
        <dd>회사소개</dd>
        <dd>연혁</dd>
        <dd>오시는 길</dd>
    </dl>
</body>
</html>
```

<br><hr><br>

## 5. 하이퍼링크 요소

- 하이퍼링크(Hyperlink) 라는 것은 단어나 기호, 그림 등을 문서 내의 다른 요소나 다른 문서로 연결해 놓은 일. 이 부분을 마우스로 클릭하면 지정된 위치로 이동하는 것을 말합니다.

<br>

### 5-1. 기본 문법

```html
<a href="내부문서URL">내부문서</a>
<a href="외부사이트URL" target="_blank">외부사이트</a>
<a href="#이동할아이디">네임앵커</a>
<a href="mailto:이메일주소">이메일보내기</a>
<a href="tel:전화번호">전화걸기</a>
<a href="sms:전화번호">문자보내기</a>
<a href="파일URL" download>다운로드</a>
<a href="javascript:함수명()">자바스크립트 실행1</a>
<a href="#" onclick="함수명()">자바스크립트 실행2</a>
```

<br>

### 5-2. 기본 예시

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>하이퍼링크 연습</title>
</head>
<body>
    <h2>하이퍼링크 요소</h2>
    <p>하이퍼링크 요소란? 해당 텍스트나 요소를 클릭하면, 다른 화면이나 페이지, 
        서비스로 이동하는 것을 말한다.</p>
    <p>a(anchor) : 앵커 -> 하이퍼링크 요소</p>
    <hr>
    <ul>
        <li><a href="ex02.html">같은 사이트 내에서 다른 페이지로 이동</a></li>
        <li><a href="https://www.naver.com" target="_blank" title="외부사이트로 이동">
            다른 사이트를 이동할 경우</a></li>
        <li><a href="#footer" title="푸터로 이동합니다.">네임앵커</a></li>
        <li><a href="mailto:kkt09072@naver.com">메일 보내기</a></li>
        <li><a href="tel:010-1234-5678">전화걸기</a></li>
        <li><a href="sms:010-1234-5678">문자 보내기</a></li>
        <li><a href="document_rule.hwp" download>다운로드</a></li>
    </ul>
    <hr>
    <div class="blank" style="height:5000px;background-color:yellow"></div>
    <div id="footer" style="background:deeppink">
        <h2>푸터</h2>
        <a href="#">위로</a>
    </div>    
</body>
</html>
```

<br><hr><br>

## 6. 미디어 관련 요소

- 미디어 관련 요소에는 img, video, audio, source, embed, object, iframe 요소가 있습니다.

<br>

### 6-1. 이미지

- img 요소는 이미지를 표시할 경우 활용되며, 기본(필수) 속성으로 이미지의 경로를 나타내는 src 속성과 이미지가 나타나지 못할 경우 대체 텍스트를 설정하는 alt 속성을 지정합니다.
- img 요소로 표현할 수 있는 이미지의 종류는 .jpg, .webp, .png, .gif 등이 있습니다.


<br>

#### 6-1-1. 이미지 요소 문법

```comment
<img src="파일이름을포함한이미지경로" alt="대체텍스트">
```

<br>

#### 6-1-2. 이미지 요소 사용 예시

```html
<img src="./images/ive.jpg" alt="아이브">
```

<br><br>

### 6-2. 오디오 요소

- audio 요소는 사운드 요소를 삽입할 경우 활용되며, 기본 속성으로 src 속성이 있지만, 웹 브라우저 마다 재생하는 코덱의 차이로 인해 제각각 지원하는 파일 형식이 다르므로, 보통 여러 타입(mp3, ogg, wav 등)의 사운드를 준비하여 source 요소의 src 속성에 지정하는 것이 일반적이며, 이는 크로스 브라우징을 위해 필요합니다.

<br>

### 6-2-1. 오디오 요소의 속성과 타입

<br>

### 6-2-2. 오디오 요소 문법

```comment
<audio [controls | autoplay | muted]>
    <source type="MIME타입" src="파일이름을포함한사운드파일경로">
    ....
</audio>
```

<br>

### 6-2-3. 오디오 요소 사용 예시


<br><br>

### 6-3. 비디오 요소

- video 요소는 동영상 요소를 삽입할 경우 활용되며, 기본 속성으로 src 속성이 있지만, 웹 브라우저 마다 재생하는 음성 코덱의 차이로 인해 제각각 지원하는 파일 형식이 달라 여러 타입(mp4, ogv, webm 등)의 동영상을 준비하여 source 요소의 src 속성에 지정하는 것이 일반적이며, 이는 크로스 브라우징을 위해 필요합니다.

<br>

#### 6-3-1. 비디오 요소의 속성과 타입

<br>

#### 6-3-2. 비디오 요소의 기본 문법

<br>

#### 6-3-3. 비디오 요소의 사용 예시

<br><br>

### 6-4. 소스 요소

- source 요소는 video나 audio 등의 부속 요소로 type 속성과 src 속성을 기본(필수) 속성을 세부사항으로 지정할 때 활용합니다.

<br>

#### 6-4-1. 소스(source) 요소를 통한 크로스 브라우징

<br><br>

### 6-5. 오브젝트(object) 요소

- object 요소는 사운드/동영상 요소를 추가할 때 활용되며, 기본(필수) 속성으로는 data 속성과 type 속성을 지정하여야 하며, HTML4에서 사용하던 방식으로 현재는 HTML5 웹 표준 문법상 크로스 브라우징 기능을 지원하지 않아 잘 사용하지 않고, video나 audio 요소를 활용하는 것이 좋습니다.

<br>

#### 6-5-1. 오브젝트 요소의 기본 문법

```
<object data="파일이름을포함한사운드파일경로" type="MIME타입">
    <param name="파라미터이름" value="true | false">
    ....
</object>
```

<br>

#### 6-5-2. 오브젝트 요소의 사용 예시

```html
<object data="./music/ive1.mp3" type="audio/mp3">
    <param name="AutoStart" value="true">
    <param name="AutoRewind" value="true">
</object>
```

<br><br>

### 6-6. 내장 요소

- embed 요소는 오디오/동영상 요소를 추가할 때 활용되며, 기본(필수) 속성으로는 data 속성과 type 속성을 지정하여야 하며, HTML4에서 사용하던 방식으로 현재는 HTML5 웹 표준 문법상 크로스 브라우징 기능을 지원하지 않아 잘 사용하지 않고, video나 audio 요소를 활용하는 것이 좋습니다.

<br>

#### 6-6-1. 내장 요소의 기본 문법

```comment
<embed src="파일명을포함한내장요소경로" [width="가로크기" | height="세로크기"]>
```

<br>

#### 6-6-2. 내장 요소의 사용 예시

```html
<embed src="./audio/ive.wma" width="560" height="313">
```

<br><br>

### 6-7. iframe 요소

<br>

#### 6-7-1. iframe 요소의 기본 문법

<br>

#### 6-7-2. iframe 요소의 사용 예시


<br><hr><br>

