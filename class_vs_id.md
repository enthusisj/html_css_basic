# 클래스 (class) 와 아이디 (id) 

## HTML 요소에게 '이름'을 주는 방법
* 클래스 (class)
* 아이디 (id)


## **클래스** (class)
* html
```html
<p class="big-blue-text">First</p>
<p>Second</p>
<p class="big-blue-text">Third</p>
```
* css
```css
.big-blue-text {
  color: blue;
  font-size: 48px;
}
```

위와 같이 코딩을 하면 결과는 밑에 사진과 같이 나온다.

![image](images/class.jpeg)   

위의 코드에서 첫 번째 ```p``` 요소와 세 번째 ```p``` 요소는 ```"big-blue-text"```라는 클래스 이름을 갖고 있다. 그러면 css에서 ```.big-blue-text```에 스타일을 입혀주면 된다. 클래스 이름이라는 걸 나타내는 '```.```(마침표)를 붙여야 한다.   

## **아이디** (id)
* html
```html
<p id="favorite-text">First</p>
<p>Second</p>
<p>Third</p>
```
* css
```css
#favorite-text {
  color: blue;
  font-size: 48px;
}
```
위와 같이 코딩을 하면 결과는 밑에 사진과 같이 나온다.   

![image](images/id.jpeg)   
위의 코드에서 첫 번째 ```p``` 요소는 ```"favorite-text"```라는 아이디를 갖고 있다. 그러면 css에서 ```#favorite-text```에 스타일을 해주었다. 클래스 이름을 나타내기 위해 '.(마침표)'를 붙인 것처럼 아이디(id)를 나타내기 위해서는 '```#```(샾 표시)'를 써줘야 한다.

# 클래스 vs 아이디
그렇다면 이 두 개의 차이점은 무엇일까?   
1. 같은 ***클래스(class)*** 이름을 여러 요소가 가질 수 있지만(**중복 가능**), 같은 ***아이디(id)*** 를 여러 요소가 **공유할 수 없다.**   
2. 한 요소가 **여러 클래스(class)** 를 가질 수 있지만, 한 요소는 **하나의 아이디(id)만** 가질 수 있다. (단, 한 요소가 클래스도 여러 개 갖고 아이디도 하나 가질 수 있다.)

