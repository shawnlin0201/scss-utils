# scss-utils
SCSS-utils 提供一些加速開發時需要的 SCSS 檔案。

# API
目前提供的檔案有：

## function.scss
- rem(targetFontPx,[rootFontSize])：自動轉換 px 至 rem。

搭配 responseTextSize.scss 實現 AWD 版面，範例：
```scss
button {
  width: rem(72px);
  height: rem(36px);
  border-radius: rem(5px);
  background:#41B883;
  color:#35495E;
  font-weight:bold;
  font-size: rem(16px);
}
```
在預設 html font-size 為 16px 的編譯結果：
```css
button {
    width: 4.5rem;
    height: 2.25rem;
    border-radius: 0.3125rem;
    background: #41B883;
    color: #35495E;
    font-weight: bold;
    font-size: 1rem;
}
```


## autoResponseTextSize.scss
根據畫面大小調整 RootFontSize，搭配 function.scss 中的 `rem()` 可快速實現 AWD 版面。

## default-font-family.scss
透過 CSS `@font-face` ，快速設定中英字型差異。
