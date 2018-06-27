# CSS in JS
`<style>`タグを生成して、`<head>`にinsertする実装パターン

多くのCSS in JSのライブラリでは擬似要素セレクタやメディアクエリ、もしくはCSSの構文そのものを使用することが出来る

# 利点
- JavaScriptから動的に変更しやすい

## 欠点
- style属性に指定できないようなスタイルを定義することが不可能、ないし困難 (疑似クラス、疑似要素、メディアクエリ)
  - できてもこの対策がツール間でまちまち

## 例
- Radium
- styled-components
  - [styled-components](https://github.com/styled-components/styled-components)
- styled-jsx
  - [堅牢なCSSをReactに手軽に実装できるstyled-jsx](https://inside.dmm.com/entry/2018/05/14/react-styled-jsx)
- Free-Style
  - [Free-Style のススメ ~ CSS Modules は解決策ではない](https://qiita.com/kimamula/items/2a5e69269e77ca85008e)
- Aphrodite
- glamor

# CSS Modules
CSSファイルからビルド時にCSSとJSが出力され、そのJSの方がimportされる

## 利点
- 実体はCSSなので、CSSで実現できることはすべて実現可能

## 欠点
- CSSとJSの間での定数の共有ができない

## 例
- css-loader
  - [webpackのcss-loaderでCSS Modulesをやる](https://qiita.com/_likr/items/c335dec5221024ad56bc)
- react-css-modules
- babel-plugin-react-css-modules

# 参考文献
- [Reactのコンポーネントのスタイリングをどうやるか](https://qiita.com/lightnet328/items/218eb1c4a347302cc340)
- [Reactと一緒に使う時のCSS in JSのライブラリ選定とか所感とか](https://qiita.com/terrierscript/items/0cfdb1a0c1d172e27694)