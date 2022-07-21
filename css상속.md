# CSS 상속
CSS에는 '상속'이라는 것이 있다. 말 그대로 부모 요소의 속성들을 자식들한테 넘겨주는 것을 말한다. 예를 들어,   

* html
```html
<div class="div1">
  <h1>Heading 1</h1>
  <p>Paragraph bla bla bla</p>
</div>
```
* css
```css
.div1 {
  color: blue;
}
```
![image](images/%EC%83%81%EC%86%8D.jpeg)    

```.div1```의 폰트 색을 blue로 설정해주었고, ```<h1>```과 ```<p>```에 대해서는 별도의 설정이 없다. 그런데도 ```<h1>```과 ```<p>``` 태그의 폰트 색이 파란색으로 설정되었다. 왜냐하면 ```.div1```의 스타일이 자식들에게 상속되었기 때문이다.

## **상속되는 속성들**

하지만, 태그와 속성에 따라 상속이 되지 않는 경우도 많이 있다. 예를 들어서 부모 태그에 설정한 ```margin```이 모든 자식들에게도 적용되면 총체적 난국이 된다.

웬만하면 상속되는 몇 가지 속성들이다.:
1. color
2. font-family
3. font-size
4. font-weight
5. line-height
6. list-style
7. text-align
8. visibility

이외에도 많지만, 일단 자주 사용하는 것들이다.

위에 있는 속성들도 항상 상속되는 것은 아니다. 대표적인 예로 ```<a>``` 태그에는 ```color``` 속성이 상속되지 않는다. ```<a>``` 태그가 억지로 상속을 받아오기 위해서는 해당 속성에 ```inherit``` 값을 쓰면 된다.

* html
```html
<div class="div1">
  Let's go to <a href="https://google.com" target="_blank">google</a>!
</div>

<div class="div2">
  Let's go to <a href="https://google.com" target="_blank">google</a>!
</div>
```
* css
```css
.div1 {
  color: green;
}

.div2 {
  color: orange;
}

.div2 a {
  color: inherit;
}
```
![image](images/%EC%83%81%EC%86%8D2.jpeg)