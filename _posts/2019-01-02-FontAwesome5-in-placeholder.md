---
layout: post
title: placeholer안에 FontAwesome5 icon 넣기
tag: etc
---

쉽게 검색해서 적용할 수 있을 줄 알았는데 생각보다 바로 안되더라..  

왜 그런가 했더니 FontAwesome이 5버전대로 올라가면서 문법이 바뀐 모양..

최근 글로 검색해봐도 제대로 적용되는 글이 한 개 밖에 없는 듯해서 나같이 헤매지 마시라고 올린다ㅋㅋ


```html
html :
<input type="text" class="fas" placeholder="&#xf002;" />
```
`placeholder="요기"` 에 넣는 코드는 <a href="https://fontawesome.com/icons?d=gallery" target="_sub">FontAwesome</a>에서 본인이 쓰고자 하는 icon을 누르면 그 icon에 해당하는 유니코드가 있다. 그 앞에 &#을 붙여서 완성하면 된다.

![search](/public/img/fa-search.png)


<br>  

이렇게만 해도 적용되는데, 혹시 placeholder안에 글씨체도 다르게 하고 싶은 분들은
```html
html :
<input type="text" placeholder="&#xf002;" />
```
```css
css :
input {
  font-size: 3rem;
  font-family: Helvetica, sans-serif;
}

input::placeholder {
  font-family: "Font Awesome 5 Free";
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  display: inline-block;
  font-style: normal;
  font-variant: normal;
  text-rendering: auto;
  line-height: 1;
  font-weight: 900;
}
```
요렇게 하면 된다  
끗.