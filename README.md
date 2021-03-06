# web2
```
css를 사용하면 디자인과 관련된 코드 중복을 제거할 수 있다!
코드 중복 제거 -> 코드 용량 ↓
태그를 지정해서 디자인 설정하니까 웹 페이지 유지 보수 쉽고 가독성이 높아짐
디자인과 관련된 코드는 <style> 태그 안에 있음

선택자 : 태그 이름 혹은 디자인을 바꾸고 싶은 태그
속성 : 태그 디자인을 어떻게 바꾸고 싶은지 설정


a {
    color:red
}

a : 선택자(selector)
color:red : 선언(declaration)
color : 속성(property)
red : 값(value)

font size 검색어 : css text size property
가운데 정렬 검색어 : css text center property

.class {

}

#id {

}

태그에 class를 여러개 적용할 수 있음. css에서 가장 나중에 선언한 클래스를 적용함.
tag -> class -> id id로 갈 수 더 우선순위 높음

▶ css selector : https://www.w3schools.com/cssref/css_selectors.asp

h1, a{
    border-width:5px;
    border-color:red;
    border-style:solid;
}
-> 위의 css를 적용하면 태그가 차지하는 공간을 알 수 있다

h1 같이 화면 전체를 차지하는 태그 : block level element ( display:block; )
p 같이 자기 자신의 크기 공간만 차지하는 태그 : inline element( display:inline; )
-> 이런 공간을 결정하는 css 속성 : display

★꿀팁?
태그를 안보이게 하고 싶을 때 -> display:none;

▶ css box model : https://www.google.co.kr/search?q=css+box+model&hl=ko&authuser=0&rlz=1C1GCEU_koKR821KR821&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjPzezc-ZTgAhUI7LwKHZSVDwUQ_AUIDigB&biw=1158&bih=592
border- 가 중복되니까 한번에 쓰고 싶을 때
h1, a{
    border:5px red solid;
}
속성에 값을 한번에 쓰자
순서는 중요하지 않음.

태그 내 content와 border 사이 값이 없으므로 공간을 주고 싶을 때 : padding
태그 border와 다른 태그 border 사이 간격 : margin
태그 내 content의 크기 : width(가로), height(세로)

div : 아무 의미가 없고 디자인의 용도로만 쓰는 태그. block level element
span : div와 같은 용도. inline element

▶ grid
div 태그를 가진 두 개의 요소들을 위 아래가 아니라 양 옆으로 배치하고 싶을 때 grid를 사용해보자
display:grid;
grid-template-columns: 150px 1fr; -> 처음 것 크기, 두번째 것 크기
fr은 화면 전체 비율을 따지는 단위(?)
그리드는 제일 위에 있는 태그 개수를 기준으로 나뉘게 됨.

★ 웹 브라우저에서 이 기술을 사용할 수 있는지 확인하는 사이트 : https://caniuse.com/

★ 반응형 디자인 : @media 쿼리
http://blog.saltfactory.net/using-css-media-query-for-responsive-web/
screen width >= 800px  
@media (min-width:800px) {}
아래와 위의 코드 의미는 같음

screen width <= 800px  
@media (max-width:800px) {}

media {} 괄호 안에 ()일 때 바꾸고 싶은 디자인 css 를 추가하면 됨.

★ css코드 재사용 -> css 파일을 만들어서 사용하고 싶은 html파일에 아래 코드를 추가함
<link rel="stylesheet" href="style.css">

★ 캐싱 : 한번 CSS파일(등 웹페이지 코드 파일들)을 저장해두면 다시 다운로드 받을 필요 없이 그 파일을 계속 사용 가능함. 다운로드 트래픽 감소 효과.
```

<strong>reference : Coding Everyday(WEB2 - CSS, creator : egoing)</strong>
<p>
https://opentutorials.org/course/3086
</p>
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3129/7333.jpg"></a>
