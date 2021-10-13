<template>
  <nav :class="headerClassList" class="fixed w-full z-30 top-0">
    <div class="header-border">
    </div>
    <div class="w-full header mx-auto flex flex-wrap items-center justify-between mt-0 py-2"
    >      
      <a
        class="inline-block login-button text-black font-bold no-underline"
        href="#"
      >
        Login
      </a>      
    </div>
  </nav>
</template>

<script>
export default {
  name: 'TheHeader',  
  data() {
    return {
      scrollY: 0,
      isOpen: false
    }
  },
  computed: {
    
  },
  methods: {
    
  },
  mounted() {
    this.scrollY = window.scrollY
    document.addEventListener('click', this.onClick)
    document.addEventListener('scroll', this.onScroll)
  },
  beforeDestroy() {
    document.removeEventListener('click', this.onClick, true)
    document.removeEventListener('scroll', this.onScroll, true)
  }
}
</script>

<style lang="css">
.login-button  {
  text-align: left;
  font: normal normal 600 14px/17px Lato;
  letter-spacing: 0.84px;
  color: #319795;
  opacity: 1;
  margin-right: 19px;
}
.header-border {
  top: 0px;
  left: 0px;
  height: 5px;
  background: transparent linear-gradient(91deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
  opacity: 1;
}
.header {
  left: 0px;
  height: 67px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  box-shadow: 0px 3px 6px #00000029;
  border-radius: 0px 0px 12px 12px;
  opacity: 1;
  justify-content: flex-end;
}
</style>
