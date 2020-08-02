<template>
  <div>
    <div>{{ ct }}</div>
    <button @click="add">jia1 </button>
  </div>
</template>

<script>
import store from "./b.js"; //export default就不用{store}了

export default{
  data(){
    var ct=store.state.count
    return {ct}
  },
  computed: {
    count () {
      return store.state.count
    }
  },
  methods:{
    add(){
     this.ct++
    }
  }
}

</script>