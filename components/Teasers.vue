<template>
  <section class="bg-white border-b py-8">
    <div class="container mx-auto flex flex-wrap pt-4 pb-12" style="justify-content: center;">
      <button
        v-for="tab in tabs"
        :key="tab"
        @click="selected = tab;"
        :class="['lg:mx-0 hover:underline text-white my-6 shadow-lg normal-button', tab, { active: selected === tab }]"
      >
        {{ tab }}
      </button>   

      <component :is="selected" class="tab"></component>   
    </div>
  </section>
</template>

<script>
import Temporärbüro from '@/components/Temporärbüro'
import Arbeitnehmer from '@/components/Arbeitnehmer'
import Arbeitgeber from '@/components/Arbeitgeber'

export default {
  name: 'Teasers',
  data: function() {
    return {
      tabs: ["Arbeitnehmer", "Arbeitgeber", "Temporärbüro"],
      selected: "Arbeitnehmer"
    };
  },
  components: {
    Arbeitnehmer,
    Arbeitgeber,
    Temporärbüro
  }
}
</script>
<style scoped>
.normal-button {
  width: 115px;
  height: 40px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  border: 1px solid #CBD5E0;  
  color: #319795;
  opacity: 1;
}
.normal-button:hover {
  text-decoration: none;
}
.normal-button:focus {
  outline: 0px;
}
.second-button {
  width: 115px;
  height: 40px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  border: 1px solid #CBD5E0;
  opacity: 1;
  color: #319795;
}
.second-button:hover {
  text-decoration: none;
}
.second-button:focus {
  outline: 0px;
}
.last-button {
  width: 115px;
  height: 40px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  border: 1px solid #CBD5E0;
  
  opacity: 1;
  color: #319795;
}
.last-button:hover {
  text-decoration: none;
}
.last-button:focus {
  outline: 0px;
}
.Arbeitnehmer {
  border-radius: 12px 0px 0px 12px;
}
.Temporärbüro{
  border-radius: 0px 12px 12px 0px;
}
.active {
  background: #81E6D9 0% 0% no-repeat padding-box;
  color: #FFFFFF;
}
</style>
