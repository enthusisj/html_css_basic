# inline-block 정리
```Block``` 요소에게는 가로 길이와 세로 길이를 직접 설정해줄 수 있다. 하지만, ```inline``` 요소는 자동으로 설정이 된다. ```Inline``` 요소는 가로, 세로 길이의 개념이 없다고 생각하면 된다.

만약, ```inline``` 요소처럼 다른 요소들과 같은 줄에 머무르면서 ```block``` 요소처럼 가로, 세로 길이도 설정해주고 싶으면 어떻게 해야 할까?    
*바로 그 둘을 섞어놓은 inline-block을 사용하면 된다.*

## **inline-block**
* html
```html
My <i>name</i> is Young!
```
* css
```css
i {
  display: inline-block;
  width: 200px;
  height: 200px;
  background-color: green;
}
```
![image](images/%EC%9D%B8%EB%B8%94.jpeg)
