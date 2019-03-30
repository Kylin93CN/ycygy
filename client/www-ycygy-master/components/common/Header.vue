<template>
  <div class="header-container">
    <div class="header-left">
      <img src="@/assets/logo/lovely-cy.png" alt="logo" class="logo" />
      <div class="love-heart">
        <div class="love">
          <span>💕</span>
        </div>
      </div>
      <div class="cygy">
        <span>超越·公益</span>
      </div>
    </div>
    
    <Navi class="header-middle" />
    <div class="header-right">
      <Button :btnName="'登陆'" />
      <Button :btnName="'注册'" />
    </div>
  </div>
</template>
<script>
import Navi from '~/components/common/Navi.vue';
import Button from '~/components/common/Button.vue';
export default {
  components: {
    Navi,
    Button
  }
}

</script>

<style scoped lang="scss">
.header-container {
  display: flex;
  height: 60px;
  width: 100%;
  background-color: #f0f6f3;
  flex-direction: row;
  .header-left {
    display: flex;
    width: 300px;
    .logo {
      width: 40px;
      margin-left: 50px;
    }
    .love-heart {
      position: absolute;
      top: 20px;
      left: 90px;
      .love {
        display: flex;
        align-items: center;
        animation: love 5s infinite;
      }
    }
    .cygy {
      margin-left: 80px;
      display: flex;
      align-items: center;
      text-shadow: #FC0 1px 0 10px;
      font-size: 20px;
      font-weight: 600;
      text-shadow: #ab4378 1px 0 10px;
      font-family: serif;
    }
  }
  .header-middle {
    display: flex;
    justify-content: flex-start;
    flex: 1;
  }
  .header-right {
    display: flex;
    width: 200px;
    margin-right: 24px;
    flex-direction: row-reverse;
  }
}

@keyframes love
{
  0% {transform:rotate(-45deg); margin-left: 0px;}
  50% {transform:rotate(45deg); margin-left: 50px;}
  100% {transform:rotate(-45deg); margin-left: 0px;}
}
</style>
