<template>
    <div class="Todos">

      <div v-bind:key="i.id" v-for="i in todos">
        <h3> {{i.title}} </h3>
      </div>
      
    </div>
</template>



<script>
export default {
  name: "Todos",
  props: ["todos"]
}
</script>



<style scoped>
  .Todos {
    margin-top: 5%;
  }
</style>