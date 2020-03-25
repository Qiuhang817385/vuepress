<template>
  <div>
    <!-- https://lokeshdhakar.com/dev-201-stripe.coms-main-navigation/
			 https://lokeshdhakar.com/dev-101-tilted-code-card/
			 -->
    <div class="space">
      <div class="card">
        <div class="card-shine"></div>
        <div class="code-snippet"><code>this is a new kai xin <br>点击链接跳转到新的页面</code></div>
      </div>
    </div>
    <br>
    <div class="space">
      <div class="card">
        <div class="card-shine"></div>
        <div class="code-snippet"><code>this is a new kai xin <br>点击链接跳转到新的页面</code></div>
      </div>
    </div>
    <br>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.space {
  perspective: 1500px;
  width: 525px;
  border-radius: 14px;
}
.car1 {
}

.card {
  display: inline-block;
  position: relative;
  border-radius: 14px;
  left: 30px;
  top: 50px;
  color: #fdfdfd;
  font-weight: 600;
  font-size: 30px;
  background: rgb(76, 171, 255);
  width: 325px;
  transform: rotate3d(0, 0, 0, 0deg) rotate(0deg);
  box-shadow: -27.1px 62.5px 125px -25px rgba(50, 50, 93, 0.5),
    -16.2px 37.5px 75px -37.5px rgba(0, 0, 0, 0.6);
}

.code-snippet {
  border-radius: 14px;
  padding: 25px 30px;
  background: url("../public/assets/1 (3).jpg") no-repeat;
  background-size: cover;
}

.card-shine {
  border-radius: 14px;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: linear-gradient(
    to top right,
    rgba(255, 255, 255, 0),
    rgba(255, 255, 255, 0) 20%,
    rgba(255, 255, 255, 0.5) 70%,
    #fff
  );
  pointer-events: none;
  opacity: 0.2;
}

/* PrismJS 1.15.0
https://prismjs.com/download.html#themes=prism-tomorrow&languages=markup+clike+javascript */
/**
 * prism.js tomorrow night eighties for JavaScript, CoffeeScript, CSS and HTML
 * Based on https://github.com/chriskempson/tomorrow-theme
 * @author Rose Pritchard
 */

code[class*="language-"],
pre[class*="language-"] {
  color: #e6ebf1;
  font-family: "Source Code Pro", Consolas, Menlo, monospace;
  font-size: 14px;
  text-align: left;
  white-space: pre;
  word-spacing: normal;
  word-break: normal;
  word-wrap: normal;
  line-height: 1.3;

  -moz-tab-size: 4;
  -o-tab-size: 4;
  tab-size: 4;

  -webkit-hyphens: none;
  -moz-hyphens: none;
  -ms-hyphens: none;
  hyphens: none;
}

.token.comment,
.token.block-comment,
.token.prolog,
.token.doctype,
.token.cdata {
  color: #999;
}

.token.punctuation {
  color: #ccc;
}

.token.tag,
.token.attr-name,
.token.namespace,
.token.deleted {
  color: #e2777a;
}

.token.function-name {
  color: #6196cc;
}

.token.boolean,
.token.number,
.token.function {
  color: #f08d49;
}

.token.property,
.token.class-name,
.token.constant,
.token.symbol {
  color: #f8c555;
}

.token.selector,
.token.important,
.token.atrule,
.token.builtin {
  color: #cc99cd;
}

.token.string,
.token.char,
.token.attr-value,
.token.regex,
.token.variable {
  color: #7ec699;
}

.token.entity,
.token.url {
  color: #67cdcc;
}

.token.important,
.token.bold {
  font-weight: bold;
}
.token.italic {
  font-style: italic;
}

.token.entity {
  cursor: help;
}

.token.inserted {
  color: green;
}

.token.function,
.token.constant,
.token.boolean {
  color: #45b2e8;
}

.token.keyword,
.token.operator {
  color: #7795f8;
}

.token.function,
.token.keyword {
  font-weight: 600;
}
</style>