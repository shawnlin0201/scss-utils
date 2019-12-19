# scss-utils
SCSS-utils 提供一些加速開發時需要的 SCSS 檔案。

# API
目前提供的檔案有：

## function.scss
- rem(targetFontPx,[rootFontSize])：自動轉換 px 至 rem。（製作 WEB mobile 版時，搭配 responseTextSize.scss 可實現 AWD 版面。）

## autoResponseTextSize.scss
根據畫面大小調整 RootFontSize，搭配 function.scss 中的 `rem()` 可快速實現 AWD 版面。

## default-font-family.scss
透過 CSS `@font-face` ，快速設定中英字型差異。
