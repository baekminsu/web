# 2주차


### HTML5 문서구조

#### HTML 태그의 특징
 - <img src="heart.jpg" width = "100" height = "50" alt = "사랑합니다"
 <br>
 있었을때 img 태그이름이고 src= 에서 "까지 속성이고 heart.jpg는 속성 값이다
 - 시작태그와 종료태그라고 부른다

#### 헤딩
- 헤딩(heading) :웹 페이지의 머리기사(headline)
<br>
 h1  /h1 으로사용하고 6까지있으면서 크기가 점차 작아진다
- title 속성으로 툴팁을 달아보자
<br>
h1 title =&lt;"h1태그로 작성하였습니다."> 1장 홈페이지 </h1&gt;
<br>
이러면 텍스트 위에 마우스를 올리면 툴팁이 출력된다.

#### 단락나누기 <p&gt; , </p&gt;
- paragraph
- 종료 태그가 있다. 단락과사이의 줄이들어간다

#### 수평선긋기 <hr&gt;
- A horizontal rule
- 이렇게 수평선 들어감
- 종료태그가 없어서 쓴즉시 밑에 들어감
<hr>

#### 새로운줄로 넘어가기 <br&gt;
- line break

#### 문자,기호,심볼 입력 <,> 기호 등
- ",',<,>,&,빈칸,파운드,루트,무한대,위화살표,나누기,시그마 등을 표현할 수 있다. 이건 ppt 확인

#### 입력한 그대로 화면에 표시하는 태그 <pre&gt; </pre&gt;
- <br&gt; 안써도 엔터를 내가 넣었으면 그대로 출력된다.

#### 텍스트 꾸미기
- <mark> 형광펜칠하자 </mark>
    - <mark&gt; </mark&gt;
- <b> 진하게 </b>
    - <b&gt; , </b&gt;
- <strong> 중요하게 </strong>
    - <strong&gt; , </strong&gt;
- <em> 강조 </em>
    - <em&gt; , </em&gt;
- <i> 이탤릭체로 강조 </i>
    - <i&gt;,</i&gt;
- 보통문자보다 <small>한문자작은 </small>
    - <small&gt; , </small&gt;
- <del> 는아니고체</del>
    - <del&gt; , </del&gt;
- <ins> 밑줄 </ins>
    - <ins&gt; , </ins&gt;
- 보통문자의 <sup>윗첨자</sup>
    - <sup&gt;,</sup&gt; 
- 보통문자의 <sub>아래첨자</sub>
    - <sub&gt;,</sub&gt;
- <code>텍스트</code>가 코드임을 표시한다
    - <code&gt; , </code.&gt;       

#### 블록 태그와 인라인 태그
- 태그 : 블록 태그와 인라인 태그로 구분
<br>
    - 블록 태그 사례 : <p&gt;, <h1&gt;,<div&gt;,<ul&gt;
    - 인라인 태그 사례 : <strong&gt;, <a&gt;,<img&gt;,<span&gt; 등
- 블록 태그 :
    - display 속성값이 블록(block)인 요소는 언제나 새로운 라인(line)에서 시작하며,해당 라인의 모든 너비를 차지
    - 블록태그로 <div&gt; 를 많이사용한다.
- 인라인 태그:
    - display 속성값이 인라인(inline)인 요소는 새로운 라인(line)에서 시작하지 않는다. 요소의 너비도 해당 라인 전체가 아닌 해당 HTML 요소의 내용 만큼만 차지 한다.
    - <span&gt; 를 주로 이용하는데 텍스트의 특정 부분을 묶는 데 자주 사용되는 인라인(inline) 요소 이다.
    주로 텍스트의 특정 부분에 따로 스타일을 적용하기 위해 사용한다.
    - 그 밖의 <a&gt;, <img&gt; 인 대표적인 요소가 있다.
- 사용 예제 :
<br>
&lt;div style="background-color:skyblue; padding:20px;"&gt;
내가 사람의 방언과 천사의 말을 할지라도
&lt;span style="color:red">사랑&lt;/span>이 없으면
소리 나는 구리와 울리는 꽹과리가 되고,
&lt;span style="color:red"&gt;사랑&lt;/span>이 없으면 아무
것도 아니라.

#### 메타 데이터 삽입

- 메타데이터
    - 데이터를 설명하는 데이터
    - HTML 문서에 &lt;meta&gt; 요소를 이용해 "공식적으로" 메타데이터를 적용할 수 있다.
        - 많은 <meta> 요소는 name과 content 속성을 가진다

        -사용 예제:
        <br>
        &lt;meta name="author" content="Chris Mills" /&gt;
        <br>
&lt;meta
    name="description"
    content="The MDN Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications."
/&gt;
- HTML 페이지에 대한 메타 데이터를 담기 위한 태그들
    - &lt;base&gt;,&lt;link&gt;,&lt;script&gt;,&lt;style&gt;,&lt;title&gt;,&lt;meta&gt;
    - &lt;base&gt; 에 대해 알아보자
        - 웹 페이지들의 기본 URL과 페이지가 출력될 윈도우 지정
        - 사용예제:
        <br>
        &lt;a href="http://www.mysite.com/score/math.html"&gt;수학&lt;/a&gt;이 있다면 이것을 아래와 코드로 수정 가능
        <br>
        &lt;head&gt;
        <br>
            &lt;base href="http://www.mysite.com/score/"&gt;
        <br>
        &lt;/head&gt;
        <br>
        ~
        <br>
        &lt;a href ="math.html"&gt;&lt;수학/a&gt; 으로 수정가능
    - &lt;link&gt; 에 대해 알아보자
        - 사용예제:
        <br>
        &lt;head&gt;
        <br>
        &lt;link type="text/css" rel="stylesheet" href="mystyle.css" &gt;
        <br>
        &lt;/head&gt;
        <br>
        ex)mystyle.css에 저장된 스타일 시트를 불러오도록 지시
    - &lt;meta&gt; 에 대해 알아보자
        - 사용예제 :
        <br>
        보통 그냥 이렇게 쓴다.
        &lt;mata name ="auther" content = "황기태" &gt; 웹페이지 저작자가 "황기태"임을 표기하는 사례이다.
        -웹페이지의 저작자, 문자 인코딩 방식,내용 등 charset 등도 익숙할것 이다.
- 페이지의 &lt;head&gt; 요소 안에 있으며, 다양한 형태의 &lt;meta&gt; 가 있다.

#### 이미지
- 이미지는 인라인 요소이다.
- &lt;img&gt; 태그 사용
    - &lt;img src="dog.jpg" width ="300" height ="230" alt ="No image&gt;
    - src 속성은 이미지 파일 이름을 지정
        - 지정할 수 있는 이미지 종류로 :BMP,GIF,PNG,JPG(JPEG),animated-GIF
    - width,height 는 속성인데 각각 이미지의 가로,세로 크기를 나타냄
    - alt는 이미지 표시안될때 화면에 표시되는 텍스트 출력
- 이미지 처리방법
    - 클라이언트에서 HTTP Request
    - 그러면 웹서버에서 HTTP Response
#### 링크
- 하이퍼링크(또는 링크)는 다른 문서로 점프할 수 있는 단어나 이미지
<br>
&lt;a href="info.html"&gt; 구글사이트 &lt;/a&gt;
    - a 링크는 다른 페이지로 링크를 생성할 때 사용
    - href 속성은 링크의 목적지를 나타냄
    - 구글사이트는 그냥 링크텍스트 화면에 밑줄 그어짐
#### 리스트 만들기
    - <ul>
        <li> ~ </li>
        <li> ~ </li>
      </ul>
    
##### 3 가지 종류의 리스트
- 순서있는리스트 : &lt;ol&gt;,&lt;/ol&gt;
    - li 할떄마다 앞에 A.,B.,C. 붙어나옴 나오는것들을 "마커"라고 부른다. (타입설정안할시) 1로설정하면 1.2.3.4.
- 순서없는리스트 : &lt;ul&gt;,&lt;ul&gt;
    - li 할떄마다 앞에 점만튀어나옴
- 정의리스트 : &lt;dl&gt;,&lt;/dl&gt;
    - &lt;dt>용어 -내어 쓰기
    - &lt;dd>설명 -들여 쓰기
    <br>
    <dl>
    <dt>에스프레소</dt>
    <dd>- 커피의 기본, 커피의 원액이다.</dd>
    <dt>아메리카노</dt>
    <dd>- 에스프레소에 물을 넣은 것</dd>
    <dt>카페라떼</dt>   
    <dd>- 커피에 우유를 섞은 것</dd>
</dl> 
    이렇게나온다

##### 리스트 아이템
- &lt;li&gt;~ &lt;/li&gt;
- &lt;/li&gt; 생략 가능

#### 표만들기
 - 표 만드는데 사용하는 태그
 <br>
 &lt;table&gt; : 표전체를 담는 컨테이너
 <br>
 &lt;caption&gt; : 표 제목
 <br>
 &lt;thead&gt; : 헤딩 셀 그룹
 <br>
 &lt;tfoot&gt; : 바닥 셀 그룹
 <br>
 &lt;tbody&gt; : 데이터 셀 그룹
 <br>
 &lt;tr&gt; : 행 (여러 &lt;td&gt;,&lt;th&gt; 포함한다
 <br>
 &lt;td&gt; : 데이터 셀

##### 예제 코드와 결과를 살펴보자
    <table border ="1"> 
	<caption>1학기 성적</caption>
	<thead>
        <tr>
            <th>thead</th><th>HTML</th><th>CSS</th>
        </tr> 
    </thead>
    <tbody>
        <tr>
            <th>tbody</th><th>80</th><th>80</th>
        </tr>
        <tr>
            <th>이재문</th><th>95</th><th>99</th>
        </tr>
        <tr>    
            <th>이병은</th><th>40</th><th>61</th>
        </tr>
    </tbody>
	<tfoot>
        <tr>
            <th>tfoot</th><th>225</th><th>230</th>
        </tr>
    </tfoot>
    <table>	
    </table>

<table border ="1"> 
	<caption>1학기 성적</caption>
	<thead>
        <tr>
            <th>thead</th><th>HTML</th><th>CSS</th>
        </tr> 
    </thead>
    <tbody>
        <tr>
            <th>tbody</th><th>80</th><th>80</th>
        </tr>
        <tr>
            <th>이재문</th><th>95</th><th>99</th>
        </tr>
        <tr>    
            <th>이병은</th><th>40</th><th>61</th>
        </tr>
    </tbody>
	<tfoot>
        <tr>
            <th>tfoot</th><th>225</th><th>230</th>
        </tr>
    </tfoot>	
</table>

##### 행과 열을 병합해보자 (코드 및 결과 colspan,rowspan 사용)
    <table border ="1"> 
	<caption>1학기 성적</caption>
        <tr>
            <th colspan ="3"> 묵었지롱</th>
        </tr>
        <tr>
            <th>이재문</th><th>95</th><th rowspan ="2">여기도묵었</th>
        </tr>
        <tr>    
            <th>이병은</th><th>40</th>
        </tr>
        <tr>
            <th>tfoot</th><th>225</th><th>230</th>
        </tr>	
    </table>
<table border ="1"> 
	<caption>1학기 성적</caption>
        <tr>
            <th colspan ="3"> 묵었지롱</th>
        </tr>
        <tr>
            <th>이재문</th><th>95</th><th rowspan ="2">여기도묵었</th>
        </tr>
        <tr>    
            <th>이병은</th><th>40</th>
        </tr>
        <tr>
            <th>tfoot</th><th>225</th><th>230</th>
        </tr>	
</table>
- 그런데 굵기조정은 border도 괜찮지만 CSS 로 하는것이 바람직하다
<br>
- 이미지들은 HTML 파일 경로아래 media 폴더에 두자 근데 media는 임의적

### 마지막 하이퍼링크 만들기
- 같은 웹 사이트에 있는 웹 페이지 연결
    - &lt;a href="picturepage.html"&gt; 클릭하면 사진 페이지로 &lt;/a&gt;
    
- 다른 웹 사이트의 웹 페이지 연결
    - &lt;a href="http://www.naver.com"&gt; 네이버 &lt;/a&gt;    
    - &lt;a href="http://www.siter.com/login.html"&gt; 사이트 로그인 &lt;/a&gt;
- 이미지 하이퍼 링크 만들기
    - &lt;a href = "http://www.naver.com"&gt;
    <img src = "naver.jpg" alt= "네이버 사이트">
    &lt;/a&gt;
- 링크 색 구분
    - 처음색은 밑줄과 함께 blue
    - 방문후면 purple
    - 누르고 있는동안은 red
    - CSS3을 이용하여 링크 색 지정 가능

### 찐막 id 속성 (동일한 페이지에서 지정하면 점프할 수 있다.)
    <a href="jump1"> 점프를 해보자 </a>
    ~
    ~
    ~
    ~
    ~
    <a id = "section"> 점프 됐다</a>
 
