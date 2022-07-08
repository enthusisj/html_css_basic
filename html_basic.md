# HTML 기초 정리 with CSS
복습을 위해 기초 정리를 해보았다.

## HTML 기본 전체 구조
```html
    <html>
        <head>
            주로 스타일, meta설정, 타이틀 적는다.
        </head>
        <body>
            그 외 내용들
        </body>
    </html>
```

## meta
 ```html
    <meta charset="utf-8">
 ```
 
 이 코드는 사파리(웹)에서 한글을 지원해주지 않으므로 한글 깨지는 것을 방지하기 위해 명령을 주는 코드이다.   

## 글 정렬
 ```css
    text-align : left; /* 왼쪽 정렬 */
    text-align : right; /* 오른쪽 정렬 */
    text-align : center; /* 가운데 정렬 */
 ```

글을 정렬 할때 쓰이는 코드이다.    

## 여백    
 **margin**  속성 사용하면 요소 사이의 여백 설정할 수 있다.   
 여백 크기는 픽셀(px)단위로 주로 쓰인다.   
 예를 들면,
 ```css
    margin-bottom: 80px;
    margin-left: 50px;
 ```

 ## 하이퍼링크(Anchor)
 하이퍼링크는 알파벳 a를 따서 ```<a>``` 태그를 쓴다.

 ```<a href="링크주소">내용</a>``` 기본 구성이다.   

 예를 들어, 
 ```html
    <a href="https://google.com" target="_blank"> 구글로가는 링크</a>
 ```

 쓰이는 데 여기서 ```target="_blank"```는 새로운 탭 열려서 구글 웹페이지를 띄워준다. 만약 안쓰게 된다면, 기존 창이 구글 창으로 바뀐다.   


 ```html
    <a href="../index.html">index</a>
 ```
 html인덱스 파일 앞에 ``..``은 상위(이전) 홈페이지 이동을 해주는 것이다.   

 두번 상위 이동을 해야한다면?   
 ```../../``` 두번 써주면 된다.    

 ## 이미지
 ```html
    <img src="링크.jpg" width="" height="">
 ```
 이미지를 코드를 쓸 때는 ```img src``` 속성을 해준다.   
 이미지 그림이 클 경우 ```width```와 ```height```를 써서 넓이 길이를 써준다.

