# scss-utils
SCSS-utils 提供一些加速開發時需要的 SCSS 檔案。

# API
目前提供的檔案有：
## _function.scss
- rem(targetFontPx,[rootFontSize])：自動轉換 px 至 rem。（製作 WEB mobile 版時，搭配 _responseTextSize.scss.scss 可實現 AWD 版面。）
## _autoResponseTextSize.scss
根據畫面大小調整 RootFontSize。
