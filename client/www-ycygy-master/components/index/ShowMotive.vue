<template>
  <div class="show-container">
    <ul>
      <li>
        <div class="show-item">
          <div class="show-content">
            <p>村花的魅力就是她开心就笑，伤心害怕就哭，想笑就笑，想哭就哭。</p>
            <p>你就像看着一个孩子，她笑了你也会感受她的喜悦，她哭时带着一股倔强。</p>
            <p>你能知道她哭后的决心，也许就是我们追求的所谓纯真。</p>
            <p class="sm">在月芽村，你可以帮助TA，或者获取TA的帮助！</p>
          </div>
          <div class="show-pic">
            <img class="show-img" src="~/assets/show/show001.png" alt="yyc">
          </div>
        </div>
      </li>
      <li>
        <div class="show-item">
          <div class="show-content">
            <p>村民们和她一样人美（帅）心善，❤支持公益正能量！</p>
            <p class="sm">画廊，展示每一次耀眼的瞬间！</p>
          </div>
          <div class="show-pic">
            <img class="show-img-half" src="~/assets/show/hl003.jpg" alt="yyc">
            <img class="show-img-half" src="~/assets/show/hl004.jpg" alt="yyc">
          </div>
        </div>
      </li>
      <li>
        <div class="show-item">
          <div class="show-content">
            <p>积分排行榜</p>
            <p class="sm">爱心有价亦无价！</p>
          </div>
          <div class="show-pic">
            <img class="show-img" src="~/assets/show/phb.jpg" alt="yyc">
          </div>
        </div>
      </li>
      <li>
        <div class="show-item">
          <div class="show-content">
            <p>关于我们</p>
             <p class="sm">我们是，不愿意透露组织的希望村团委！</p>
          </div>
          <div class="show-pic">
            <img class="show-img" src="~/assets/show/show001.png" alt="yyc">
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'ShowMotive',
}
</script>
<style scoped lang="scss">

@mixin half-content {
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
};
.show-container {
  width: 100%;
  ul {
    list-style: none;
    li {
      list-style: none;
      height: 400px;
      background-image: radial-gradient(farthest-corner at 20% 20%, #0c7575, #7171B7);
    }
  }
  .show-item {
    height: 100%;
    display: flex;
    flex-direction: row;
    .show-content {
      @include half-content;
      flex-direction: column;
      p {
        text-shadow: #ff07f7 1px 0 10px;
        padding: 5px;
        color: #fff;
      }
      .sm {
        text-shadow: #e50dff 1px 0 10px;
        padding-top: 70px;
        font-size: 21px;
      }
    }
    .show-pic {
      @include half-content;
      .show-img {
        width: 100%;
        height: 350px;
        padding: 3%;
        filter: drop-shadow(5px 5px 5px #333);
      }
      .show-img-half {
        padding: 3%;
        width: 50%;
        height: 350px;
        filter: drop-shadow(5px 5px 5px #333);
      }
    }
  }
}
</style>
