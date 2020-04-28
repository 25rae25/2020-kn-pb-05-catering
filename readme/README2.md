 # HTML, CSS 정리
 ## Block, Inline 요소
 ### Block - 영역을 가진다(한줄)
1. h1 ~ h6 : Headline태그(숫자가 작을수록 크다. 기본 Bold체)
2. div : 기본이되는 Block요소(속성이 없다.)
3. p : 문단을 나눌때 쓴다.
### Inline - 글씨로 취급된다.
1. span: 기본이 되는 Inline요소(속성이 없다.)
2. a: Anchor 링크를 표현한다.
```html
<a href="./p1.html"><!-- 현재창열기 -->
<a href="./p1.html" target="blank"><!-- 새창열기 -->
```
3. img: 이미지를 표현한다.
```html
<img src="../img/p1.jpg" alt="이미지1">
```

## CSS 기본
### Text와 관련된것 
1. color : 글씨 색상
2. text-align : 정렬(center, **left**, right, justify)
3. font-size : 글씨 크기(**12px, 16px**)
### 여백과 관련된 것
1. margin: 바깥쪽 여백
2. padding: 안쪽 여백
```css
div {margin: 0} /* 상하좌우 */
div {margin: 20px 0} /* 상하(20px) 좌우(0)*/
div {margin: 10px 20px 30px 40px} /* 상(10)우(20)하(30)좌(40) */
```
### 배경과 관련된 것
1. background-color: 배경색
```css
div {background-color: red;}
div {background-color: #ff0000;}
div {background-color: hsl(0, 100%, 100%);}
div {background-color: rgb(255, 0, 0);}
div {color: rgb(255, 0, 0);}
div {color: rgb(255, 0, 0);}
div {color: hsl(0, 100%, 100%);}
div {color: rgb(255, 0, 0);}
```
### 선택자
1. 태그선택자
```css
div{color: red;}
h1{color: red;}
```
2. 쿨래스 선택자
```html
<div class="my"></div>
```

```csss
.my {color: red;}
```
3. 아이디 선택자
```html
<div class="my"></div>
```

```css
#my {color: red;}
```

4. 자식(자손) 선택자
```html
<div class="wrap">
	 <p>
		 <div>아버지를 아버지라...</div>
		 <img src="./img/hong.jpg" alt=홍길동">
   </p>
</div>
```

```css
#my {color: red;}