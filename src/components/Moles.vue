<template>
   <div class="mole-container">
      <div class="mole">{{ moles[0] }}</div>
      <div class="mole">{{ moles[1] }}</div>
      <div class="mole">{{ moles[2] }}</div>
      <div class="mole">{{ moles[3] }}</div>
   </div>
</template>

<script>
export default {
   name: 'Moles',
   data: () => {
      return {
         moles: [false, false, false, false]
      };
   },
   props: ['moleData']
}
</script>

<style>

</style>
