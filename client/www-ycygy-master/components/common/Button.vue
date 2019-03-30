<template>
  <a class="colorful-btn">{{btnName}}</a>
</template>
<script>
export default {
  name: 'Button',
  props: ['btnName']
}
</script>

<style scoped lang="scss">
.colorful-btn {
    padding: 10px;
    color: lightslategray;
    text-transform: uppercase;
    // background: linear-gradient(135deg, #e570e7 0%,#79f1fc 100%);
    text-align: center;
    box-shadow: 0 2px 3px rgba(0, 0, 0, 0.3);
    cursor: pointer;
    text-decoration: none;
    -webkit-tap-highlight-color: transparent;
    border-radius: 5px;
    margin: 15px;
    line-height: 10px;
    font-family: roboto, helvetica;
    letter-spacing: 5px;
}
</style>
