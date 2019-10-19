# css-anti-pattern

## subTitle

HTMLなど詳細度の高い要素にCSSを反映しない。

**main** -- bad code

``` SCSS
h2 {
    foo: bar;
}

div {
    p {
        foo: bar;
    }
}
```
## subTitle

**main** -- bad code

``` CSS
h2 {
    foo: bar;
}
```

**main** -- good code

``` CSS
h1, h2, h3 {
    foo: bar;
}
```