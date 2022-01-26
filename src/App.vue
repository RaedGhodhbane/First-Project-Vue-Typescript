<template>
<div class="app">
  <p> {{jobs[0].location}}</p>

</div>
</template>

<script lang="ts">

import { defineComponent, reactive, ref, toRefs } from 'vue';
import Job from './types/Job'


export default defineComponent({
  name: 'App',
  components: {},
  setup() {
    // const state = reactive({
    //   name : 'Link',
    //   age: 25 as string | number

    // })

    // state.name = 'Shaun' 
    // state.age = '26'

    // return { ...toRefs(state)}

    // const name = ref('Link')
    // const age = ref<number | string>(25)

    // return { name, age}

  const jobs = ref<Job[]>([
    { title: 'farm worker',location:'lon lon ranch', salary: 30000, id:'1'},
    { title: 'farm worker',location:'lon lon ranch', salary: 30000, id:'2'}
  ])
    return {jobs}
  }
});
</script>

<style>

</style>

