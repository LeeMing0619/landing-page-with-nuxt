<template>
  <div class="pt-24">
    <div
      class="container mx-auto flex flex-wrap flex-col md:flex-row items-center"
    >
      <!--Left Col-->
      <div
        class="flex flex-col w-full md:w-2/5 justify-center items-start text-center md:text-left"
      >
        <h1 class="my-4 text-5xl font-bold leading-tight">
          Deine Job website
        </h1>
      </div>
      <!--Right Col-->
      <div class="w-full md:w-3/5 py-6 text-center">
        <img class="w-full md:w-4/5 z-50" src="~/assets/img/agreement.png" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroContent'
}
</script>
<style>
.pt-24 {
  top: 0px;
  left: -137.22900390625px;
  height: 659px;
  background: transparent linear-gradient(141deg, #EBF4FF 0%, #E6FFFA 100%) 0% 0% no-repeat padding-box;
  opacity: 1;
}
.my-4 {
  top: 90px;  
  height: 100px;
  text-align: center;
  font: normal normal medium 42px/50px Lato;
  letter-spacing: 1.26px;
  color: #2D3748;
  opacity: 1;
}
</style>
