# Nomadcoders Kokoa Clone Update

### margin-collapsing(마진 상쇄)

block 요소간의 margin이 겹칠 때 상하여백이 상쇄되어 두 요소의 margin값이 더해지는 것이 아니라 한 쪽 값만 적용되는 현상.

(참고: [https://velog.io/@raram2/CSS-마진-상쇄Margin-collapsing-원리-완벽-이해](https://velog.io/@raram2/CSS-%EB%A7%88%EC%A7%84-%EC%83%81%EC%87%84Margin-collapsing-%EC%9B%90%EB%A6%AC-%EC%99%84%EB%B2%BD-%EC%9D%B4%ED%95%B4))

```html
<head>
    <title>The Korea Times</title>
    <style>
        html {
            background-color: tomato;
        }
        body {
            margin: 20px 10px;
            background-color: thistle;
        }
        div {
            margin: 30px 15px;
            height: 150px;
            width: 150px;
            background-color: whitesmoke;
        }
    </style>
</head>
<body>
    <div></div>
</body>
```

이 경우, `<body>`와 `<div>`의 상하 마진은 더해진 50px이 아니라 30px가 적용된다.

### BEM (Block, Element, Modifier)

HTML과 CSS에서 클래스명을 짓는 방법 중 하나. 쉽게 보자면 자식은 ‘\_\_’ 속성은 ‘—’로 구분한다.

```jsx
<a class="btn btn--big btn--orange" href="https://css-tricks.com">
    <span class="btn__price">$9.99</span>
    <span class="btn__text">Subscribe</span>
</a>
```

참고: [https://css-tricks.com/bem-101/,](https://css-tricks.com/bem-101/) [https://nykim.work/15](https://nykim.work/15)

### display: flex; 총정리

참고: [https://studiomeal.com/archives/197](https://studiomeal.com/archives/197)

### will-change

적용할 애니메이션을 브라우저에게 미리 알려주어 최적화해서 보여주도록 함.

참고: [https://developer.mozilla.org/ko/docs/Web/CSS/will-change](https://developer.mozilla.org/ko/docs/Web/CSS/will-change)
