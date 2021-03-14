# TheMusicians
# HTML 기초 1

## 1. TAG  란?

테그란 웹 문서에서 어떤 표시를 해주는 것이라고 생각할 수 있다.

```html
<strong>Michael <u>Joseph</u> Jackson (August 29, 1958 – June 25, 2009)</strong>
```

마이클 잭슨 이름에 강조표시가 들어가고 미들네임에는 밑줄까지 들어갔다.

### 1.1. 주요 태그

```html
<h1>HTML</h1>
<p>lolem</p>
<strong>Michael</strong>
<u>Joseph</u>
<br>줄바꿈 코드이고 닫힘 코드를 따로 안 쓴다.
```



### 1.2. 기본 CSS 태그

```html
<p style="margin-top:45px;">HTML elements are </p>
```

style코드를 추가하여 줄 간격을 45px만큼 하였다.

**CSS는 기본 주제가 아니니 크게 신경x**

#### 정리

기본적으로 br태그로 많이 쓰이지만 p태그가 더 선호된다.

CSS태그를 추가하여 조금 더 세밀하게 꾸밀 수 있다.

### 1.3. 속성

속성을 이용하여 이미지 등을 추가할 수 있다.

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>Michael Jackson</h1>
    <p>
<strong>Michael <u>Joseph</u> Jackson (August 29, 1958 – June 25, 2009)</strong> was an American singer, songwriter, and dancer. Dubbed the "King of Pop", he is regarded as one of the most significant cultural figures of the 20th century.
    </p>
    <p style="margin-top:45px;">
Through stage and video performances, he popularized complicated dance moves such as the moonwalk, to which he gave the name, and the robot. His sound and style have influenced artists of various genres, and his contributions to music, dance, and fashion, along with his publicized personal life, made him a global figure in popular culture.
    </p>
    <img src="./img/Michael jackson1.jpg" width="100%">
  </body>
</html>
```

scr 부분을 주목해보다. ./ 로 디렉토리 경로를 지정하여 img폴더에 있는 이미지를 불러웠다.

### 1.4. 부모 자식 코드

아래의 코드는 li 코드를 ol(ordered list) 라는 부모코드로 감싸서 자동적으로 1, 2, 3 ... 이렇게 숫자가 붙는다.

```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```



아래의 코드는 ul 코드가 부모 코드이기 때문에 숫자가 붙지 않는다.

```html
<ul>
  <li>1. HTML</li>
  <li>2. CSS</li>
  <li>3. JavaScript</li>
</ul>
```

## 2. 문서의 구조

문장이 모여 페이지가 되고 페이지가 모여 책이 된다. 이렇게 웹 페이지가 모여서 하나의 웹 사이트가 된다. 이처럼 웹 페이지가 수 많이 모이게 되면 우리는 이를 구분 시켜야 한다. 그러기 위해 우리는 페이지마다 제목을 부여하는데 title 코드를 이용하여 정보를 잘 정리 정돈하기 위한 체계화 시킬 수 있다.

```html
<title>WEB1 - html</title>
<meta charset="utf-8">
```

메타 태그는 문자열을 똑바로 출력하도록 도와주는 코드라고 보면 된다. 요즘에는 html코드에 기본적으로 탑재가 되어있다. 

### 2.1. 링크

웹 페이지 하면 직관적으로 페이지 링크가 필요하다고 느낀다.

```html
<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 specification">Hypertext Markup Language (HTML)</a>
```

a는 anchor의 약자이고, href는 **H**yperText **Ref**erence의 약자이다. target 에 들어있는 _blank 속성은 링크를 클릭했을 때 새 창에서 페이지가 열리게 한다.

#### 2.1.1. 메인 페이지

index.html 파일을 만들어 기본 페이지를 만들것이다.

1.html은 마이클 잭슨,

2.html은 커트 코베인,

3.html은 제프 버클리로 만들것이다.

각 항목마다 링크가 달려있다. index.html 파일의 타이틀은 The greatest Musician 으로 할 것이다.

먼저 아직 밑에 나와있는1.html 밖에 없다. 그래서 나머지 페이지를 새로 만들어야한다.

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>마이클 잭슨</title>
  </head>
  <body>
    <h1><a href="index.html">The greatest Musician</a></h1>
    <ol>
      <li><a href="1.html">Michael Jackson</a></li>
      <li><a href="2.html">Kurt Cobain</a></li>
      <li><a href="3.html">Jeff Buckley</a></li>
    </ol>
    <h2>Michael Jackson</h2>
    <p><a href="https://en.wikipedia.org/wiki/Michael_Jackson" target="_blank">마이클 잭슨 위키피디아</a></p>
    <p>
<strong>Michael <u>Joseph</u> Jackson (August 29, 1958 – June 25, 2009)</strong> was an American singer, songwriter, and dancer. Dubbed the "King of Pop", he is regarded as one of the most significant cultural figures of the 20th century.
    </p>
    <p style="margin-top:45px;">
Through stage and video performances, he popularized complicated dance moves such as the moonwalk, to which he gave the name, and the robot. His sound and style have influenced artists of various genres, and his contributions to music, dance, and fashion, along with his publicized personal life, made him a global figure in popular culture.
    </p>
    <img src="./img/Michael jackson1.jpg" width="100%">
  </body>
</html>

```

그리고 지금 이 페이지에서 필요한 링크와 상단 리스트를 만들어보았다. 이를 토대로 나머지 페이지도 만들 수 있다.



## 3. 웹 페이지

다음과 같이 총 4개의 페이지를 만들어 하나의 소규모 사이트로 편성했다.

#### index.html

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>위대한 뮤지션</title>
  </head>
  <body>
    <h1><a href="index.html">The greatest Musician</a></h1>
    <ol>
      <li><a href="1.html">Michael Jackson</a></li>
      <li><a href="2.html">Kurt Cobain</a></li>
      <li><a href="3.html">Jeff Buckley</a></li>
    </ol>
    <h2>위대한 뮤지션 세 명을 소개한다.</h2>
    <p>
      <img src="./img/Michael jackson1.jpg" width="100%">
    </p>
    <p>
      <img src="./img/3kurt.jpg" width="100%">
    </p>
    <p>
      <img src="./img/2jeff.jpg" width="100%">
    </p>
  </body>
</html>

```

#### 1.html

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>마이클 잭슨</title>
  </head>
  <body>
    <h1><a href="index.html">The greatest Musician</a></h1>
    <ol>
      <li><a href="1.html">Michael Jackson</a></li>
      <li><a href="2.html">Kurt Cobain</a></li>
      <li><a href="3.html">Jeff Buckley</a></li>
    </ol>
    <h2>Michael Jackson</h2>
    <p><a href="https://en.wikipedia.org/wiki/Michael_Jackson" target="_blank">마이클 잭슨 위키피디아</a></p>
    <p>
<strong>Michael <u>Joseph</u> Jackson (August 29, 1958 – June 25, 2009)</strong> was an American singer, songwriter, and dancer. Dubbed the "King of Pop", he is regarded as one of the most significant cultural figures of the 20th century.
    </p>
    <p style="margin-top:45px;">
Through stage and video performances, he popularized complicated dance moves such as the moonwalk, to which he gave the name, and the robot. His sound and style have influenced artists of various genres, and his contributions to music, dance, and fashion, along with his publicized personal life, made him a global figure in popular culture.
    </p>
    <img src="./img/Michael jackson1.jpg" width="100%">
  </body>
</html>
```

#### 2.html

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>커트 코베인</title>
  </head>
  <body>
    <h1><a href="index.html">The greatest Musician</a></h1>
    <ol>
      <li><a href="1.html">Michael Jackson</a></li>
      <li><a href="2.html">Kurt Cobain</a></li>
      <li><a href="3.html">Jeff Buckley</a></li>
    </ol>
    <h2>Kurt Cobain</h2>
    <p><a href="https://en.wikipedia.org/wiki/Kurt_Cobain" target="_blank">커트 코베인 위키피디아</a></p>
    <p>
      <strong>Kurt Donald Cobain</strong> (February 20, 1967 – April 5, 1994) was an American singer-songwriter and musician, best known as the guitarist, primary songwriter and frontman of the rock band Nirvana.
    </p>
      Through his angst-fueled songwriting and anti-establishment persona, Cobain's compositions widened the thematic conventions of mainstream rock music. He was often heralded as a spokesman of Generation X and is considered to be one of the most influential musicians in the history of alternative rock.
    </p>
    <img src="./img/3kurt.jpg" width="100%">
  </body>
</html>

```

#### 3.html

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>제프 버클리</title>
  </head>
  <body>
    <h1><a href="index.html">The greatest Musician</a></h1>
    <ol>
      <li><a href="1.html">Michael Jackson</a></li>
      <li><a href="2.html">Kurt Cobain</a></li>
      <li><a href="3.html">Jeff Buckley</a></li>
    </ol>
    <h2>Jeff Buckley</h2>
    <p><a href="https://en.wikipedia.org/wiki/Jeff_Buckley" target="_blank">제프 버클리 위키피디아</a></p>
    <p>
      <strong>Jeffrey Scott Buckley</strong> (November 17, 1966 – May 29, 1997), raised as Scott Moorhead, was an American singer, songwriter and guitarist. After a decade as a session guitarist in Los Angeles, Buckley amassed a following in the early 1990s by playing cover songs at venues in Manhattan's East Village such as Sin-é, gradually focusing more on his own material.
    </p>
      After rebuffing much interest from record labels and Herb Cohen, the manager of his father, singer Tim Buckley, he signed with Columbia, recruited a band, and recorded what would be his only studio album, Grace, in 1994.
    </p>
    <img src="./img/2jeff.jpg" width="100%">
  </body>
</html>

```

### 완성


