<template>
  <h3>This is jobs</h3>
  <div v-for="data in datas" :key="data.id">
        <router-link :to="{name:'jobdetail', params:{id:data.id}}">
            {{ data.name }}
        </router-link>
  </div>
</template>

<script>
export default {
    data(){
        return {
            "datas" : [
                {
                    id : "1",
                    name : "Min Min Thwya",
                    job : "Developer"
                },
                 {
                    id : "2",
                    name : "Min Thwya",
                    job : "Designer"
                },
                 {
                    id : "3",
                    name : "Aung Min THway",
                    job : "Moblie"
                }
            ]
        }
    }
}
</script>

<style>

</style>