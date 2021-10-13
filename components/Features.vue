<template>
  <section class="bg-white border-b">
    <div class="container max-w-5xl mx-auto">      
      <div class="w-full">
        <div
          class="h-1 mx-auto registrienren opacity-25 my-0 py-0 rounded-t"
        >
          <button
            class="mx-auto lg:mx-0 hover:underline text-white font-bold rounded-full my-6 px-8 shadow-lg register-button"
          >
            Kostenlos Registrieren
          </button>
        </div>
      </div>      
    </div>
  </section>
</template>

<script>
export default {
  name: 'Features',  
}
</script>
<style scoped>
.registrienren {
  height: 128px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  box-shadow: 0px -1px 3px #00000033;
  border-radius: 12px 12px 0px 0px;
  opacity: 1;
  display: flex;
}
.register-button {  
  width: 320px;
  height: 40px;
  background: transparent linear-gradient(95deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
  border-radius: 12px;
  opacity: 1;
  justify-content: center;
}
</style>
