<template>
  <div class="yyc-container">
    <div id="title">
      <p><a href="#">
        第一届超越杯编程比赛
      </a></p>
    </div>
    <div class="cyb">
      <div class="loader font1">
        <span>希</span>
        <span class="span2">望</span>
        <span class="span3">村</span>
        <span class="span4">团</span>
        <span class="span5">委</span>
        <span class="span6"></span>
      </div>
    </div>
    <div></div>
    <div class="members-introduction">
      <dl>
        <dt>
          队长： Kylin
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
          队员： 金nono
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
          队员： 生生
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
          队员： liuliu
        </dt>
        <dd>
          <a href="https://weibo.com/u/5644764907">杨超越新浪微博</a>
        </dd>
        <dd>
          <a href="https://s.weibo.com/weibo/%2523%25E6%259D%25A8%25E8%25B6%2585%25E8%25B6%258A%25E5%2585%25AC%25E7%259B%258A?topnav=1&wvr=6&b=1">杨超越新浪公益话题</a>
        </dd>
      </dl>
    </div>
    
  </div>
</template>
<script>
export default {
}
</script>

<style scoped lang="scss">
$bg-color: #e0eff7;
$neon-color: rgb(103, 194, 103);
@mixin font-color {
  text-shadow: #067b96 1px 0 10px;
  color: #212018;
}
.yyc-container {
  #title{
    padding: 40px 0;
    width: 100%;
    margin: auto;
    background-color: $bg-color;
    p {
      text-align: center;
      font-size: 5em;
    }
    a {
      text-decoration:none; 
      -webkit-transition: all 0.5s;
      -moz-transition: all 0.5s;
      transition: all 0.5s;
    }

    p:nth-child(1) a {
      color:#1ea2ca;
      font-size: 0.8em;
    }
    p:nth-child(1) a:hover {
      animation: neon 1.5s ease-in-out infinite alternate; 
    }
  }
  // 超越杯
  .cyb {
    width: 100%;
    height: 100px;
    background-color: $bg-color;
    display: flex;
    justify-content: center;
    .loader {
      overflow: hidden;
      font-size: 45px;
    }
    .loader span {
      -moz-animation: loading 1s linear infinite -0.8s;
      -webkit-animation: loading 1s linear infinite -0.8s;
      animation: loading 1s linear infinite -0.8s;
      float: left;
    }
    .loader .span2 {
      -moz-animation: loading 1s linear infinite -0.2s;
      -webkit-animation: loading 1s linear infinite -0.2s;
      animation: loading 1s linear infinite -0.2s;
    }
    .loader .span3 {
      -moz-animation: loading 1s linear infinite -0.5s;
      -webkit-animation: loading 1s linear infinite -0.5s;
      animation: loading 1s linear infinite -0.5s;
    }
    .loader .span4 {
      -moz-animation: loading 1s linear infinite -1.1s;
      -webkit-animation: loading 1s linear infinite -1.1s;
      animation: loading 1s linear infinite -1.1s;
    }
    .loader .span5 {
      -moz-animation: loading 1s linear infinite -0.36s;
      -webkit-animation: loading 1s linear infinite -0.36s;
      animation: loading 1s linear infinite -0.36s;
    }
    .loader .span6 {
      -moz-animation: loading 1s linear infinite -0.65s;
      -webkit-animation: loading 1s linear infinite -0.65s;
      animation: loading 1s linear infinite -0.65s;
    }
    .loader .span7 {
      -moz-animation: loading 1s linear infinite -0.93s;
      -webkit-animation: loading 1s linear infinite -0.93s;
      animation: loading 1s linear infinite -0.93s;
    }
    .font1 {
      font-family: "Helvetica", Arial, sans-serif;
    }
  }

  .members-introduction {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    background-color: $bg-color;
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
}

@keyframes loading {
  0%, 100% {
    -moz-transform: scale(1) rotateZ(0deg);
    -ms-transform: scale(1) rotateZ(0deg);
    -webkit-transform: scale(1) rotateZ(0deg);
    transform: scale(1) rotateZ(0deg);
    opacity: 1;
  }

  26% {
    -moz-transform: scale(1.1) rotateZ(12deg);
    -ms-transform: scale(1.1) rotateZ(12deg);
    -webkit-transform: scale(1.1) rotateZ(12deg);
    transform: scale(1.1) rotateZ(12deg);
    opacity: .2;
  }

  76% {
    -moz-transform: scale(0.8) rotateZ(-8deg);
    -ms-transform: scale(0.8) rotateZ(-8deg);
    -webkit-transform: scale(0.8) rotateZ(-8deg);
    transform: scale(0.8) rotateZ(-8deg);
    opacity: .6;
  }
}

@keyframes neon {
  from {
    text-shadow: 0 0 10px #fff,
                 0 0 20px  #fff,
                 0 0 30px  #fff,
                 0 0 40px  $neon-color,
                 0 0 70px  $neon-color,
                 0 0 80px  $neon-color,
                 0 0 100px $neon-color,
                 0 0 150px $neon-color;
  }
  to {
    text-shadow: 0 0 5px #fff,
                 0 0 10px #fff,
                 0 0 15px #fff,
                 0 0 20px $neon-color,
                 0 0 35px $neon-color,
                 0 0 40px $neon-color,
                 0 0 50px $neon-color,
                 0 0 75px $neon-color;
  }
}

</style>
