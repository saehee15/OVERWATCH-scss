SCSS
### 주석
#### /* background-color: orange; */ CSS로 컴파일시 남아있음
#### // 은 CSS로 컴파일시 없어짐

---
### & : 상위 선택자 참조
---
### 변수: $로 표시
#### EX) $size: 200px
---
### 산술 연산자 나누기 / 안됨
---
#### 변수 $size: 200px 에 해당크기를 담아서 사용 or ( 30px / 2) 괄호사용
---
### 재활용 @mixin center, @include
---
#### SCSS 리팩토링
### 반복문
#### @for $i from 1 through 32 {
#### &:nth-child(#{$i}) .image{
#### background-image: url("./images/hero#{$i}.png");
#### }
---
### list와 map 은 반복문 @each
#### $list: orange, pink, yellow;
#### $map: (o: orange,p: pinky: yellow)
#### @each $c in $list {
#### .box{color: $c;}
#### }
#### @each $K, $v in $map{
#### .box-#{$k} {color: $v;}
#### }
---
### @content
