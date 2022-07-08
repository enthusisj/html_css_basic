# 스타일을 적용하는 방법
HTML 코드에 스타일을 입히는 방법에는 세 가지 있다.

## 1. ``<style>`` 태그
html
```html
<style> /* style 태그 */
  h1 {
    color: green;
    text-align: center;
  }

  p {
    font-size: 18px;
  }
</style>

<h1>Hello World!</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque sit amet lorem sit amet nunc ornare convallis. Pellentesque ac posuere lectus. In eu ipsum et quam finibus fermentum vitae sit amet magna.</p>
```

## 2. **style** 속성   
html

```html
<h1 style="color: green; text-align: center;">Hello World!</h1>
<p style="font-size: 18px;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque sit amet lorem sit amet nunc ornare convallis. Pellentesque ac posuere lectus. In eu ipsum et quam finibus fermentum vitae sit amet magna.</p>
```

## 3. 외부 **CSS** 파일 + <link> 태그
css
```css
h1 {
  color: green;
  text-align: center;
}

p {
  font-size: 18px;
}
```

html
```html
<link href="css/styles.css" rel="stylesheet">

<h1>Hello World!</h1>
```

css파일을 쓰려면 html파일에 링크를 달아서 연결해줘야 한다.   
```<link href="폴더명(폴더없으면 생략)/파일명.css" rel="stylesheet">``` 




# 어떤 방법이 효율 적일까?
일반적으로는 외부 CSS 파일에 스타일을 쓰고 HTML 코드에서 ```<link>``` 태그로 연결해주는 것이 가장 좋은 방식이다.     
하지만 조금씩 새로운 스타일을 시도해볼 때에는 간편함을 위해서 ```<style>```태그를 쓰는 방법 또는 ```style 속성```에서 테스트를 하고, 나중에 외부 CSS 파일로 옮기는 방법도 있습니다!

