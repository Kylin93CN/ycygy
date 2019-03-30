<template>
  <div class="navi-container">
    <ul>
      <li>
        <a href="/" class="navi-btn">首页</a>
      </li>
      <li>
        <a href="/yyc" class="navi-btn">月芽村</a>
      </li>
      <li>
        <a href="/gallery" class="navi-btn">画廊</a>
      </li>
      <li>
        <a href="/about" class="navi-btn">关于我们</a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
.navi-container {
    width: 600px;
    ul {
        list-style: none;
        display: inline;
        li {
            float: left;
            height: 57px;
        }
        .navi-btn {
            width: 60px;
            height: 45px;
            outline: none;
            padding: 10px;
            color: steelblue;
            text-transform: uppercase;
            text-align: center;
            cursor: pointer;
            text-decoration: none;
            -webkit-tap-highlight-color: transparent;
            border-radius: 5px;
            margin: 15px;
            line-height: 60px;
            font-family: roboto, helvetica;
            &:hover {
               background: linear-gradient(135deg, #cdb6ce 0%, #95e5ec 100%)
            }
        }
    }
}
</style>
