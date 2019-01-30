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

css selector : https://www.w3schools.com/cssref/css_selectors.asp

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

border- 가 중복되니까 한번에 쓰고 싶을 때
h1, a{
    border:5px red solid;
}
속성에 값을 한번에 쓰자
순서는 중요하지 않음.

```

<strong>reference : Coding Everyday(WEB2 - CSS, creator : egoing)</strong>
<p>
https://opentutorials.org/course/3086
</p>
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3129/7333.jpg"></a>
