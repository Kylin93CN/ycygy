<template>
  <div class="footer-container">
    <dl>
      <dt>
        友情链接
      </dt>
      <dd>
        <a href="https://weibo.com/u/5644764907">杨超越新浪微博</a>
      </dd>
      <dd>
        <a href="https://s.weibo.com/weibo/%2523%25E6%259D%25A8%25E8%25B6%2585%25E8%25B6%258A%25E5%2585%25AC%25E7%259B%258A?topnav=1&wvr=6&b=1">杨超越新浪公益话题</a>
      </dd>
    </dl>
    <dl>
      <dt>
        站点导航
      </dt>
      <dd>
        <a href="/">首页</a>
      </dd>
      <dd>
        <a href="/ycc">月芽村</a>
      </dd>
      <dd>
        <a href="/gallery">画廊</a>
      </dd>
      <dd>
        <a href="/about">关于我们</a>
      </dd>
    </dl>
    <dl>
      <dt>
        联系我们
      </dt>
      <dd>
        <span>商务合作：</span>business@ycygy.cn
      </dd>
      <dd>
        <span>帮助服务：</span>service@ycygy.cn
      </dd>
    </dl>
    
  </div>
</template>
<script>
export default {
}
</script>

<style scoped lang="scss">
@mixin font-color {
  text-shadow: #067b96 1px 0 10px;
  color: #212018;
}
.footer-container {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 100%;
  // height: 200px;
  background-color: #3a889a;
  padding: 4% 20% 2% 20%;
  color: white;
  dt {
    padding: 10px 0;
    font-size: 20px;
  }
  dd {
    padding: 10px 0;
    @include font-color;
    text-shadow: #067b96 1px 0 10px;
    span {
      width: 90px;
      text-align: center;
    }
    a {
      @include font-color;
      text-shadow: #067b96 1px 0 10px;
      text-decoration: none;
      &:visited {
        @include font-color;
      }
    }
  }
    
}
</style>
