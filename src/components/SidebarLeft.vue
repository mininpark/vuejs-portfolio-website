<template>
  <div class="SidebarLeft">
    <div class="SidebarLeft__track">
      <a href="" class="SidebarLeft__track--content">&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SidebarLeft',
  
}
</script>

<style lang="scss">
a {
  text-decoration: none;
  color: red;
}
.SidebarLeft {
  transform: rotate(270deg);
  transform-origin: left top;
  font-size: 1.5rem; 
  position: fixed; 
  }
 .SidebarLeft__track {
  position: absolute;
  white-space: nowrap;
  will-change: transform;
  animation: marquee-left 60s linear infinite; 
  }

@keyframes marquee-left {
  from { transform: translateX(-50%); }
  to { transform: translateX(-100%); }
}

</style>