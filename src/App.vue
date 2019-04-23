<template>
  <main class="row">
    <Logo />
    <p class="col-12"> Comming soon !</p>
    <div class="wave"></div>
    <div class="wave wave-bottom"></div>
  </main>
</template>

<script>
import Logo from './components/Logotipo.vue'

export default {
  name: 'app',
  components: {
    Logo
  }
}
</script>
<style lang="scss">
  @import "./assets/scss/modelo.scss";

.wave {
 width: 236%;
  height: 2900px;
  position: absolute;
  top: -25%;
  left: 50%;
  border-radius: 35%;
  background: rgba(255, 255, 255, 0.364);
  animation: wave 15s infinite linear;
  
  &-bottom{
    top: auto;
    bottom: -62px;
  }
}

@keyframes wave {
  from { transform: rotate(0deg);}
  from { transform: rotate(360deg);}
}

</style>
