<template lang="pug">
  comphead
    input.fw-input(v-model="search")
    div
      .tb-entry(v-for="v,k in animaldata.fische" v-if="search.length==0 | v.Name.toLowerCase().indexOf(search.toLowerCase())!==-1") 
        .typ Fisch
        .name {{v.Name}}
        .price 
          span {{v.Verkaufspreis}}
          span.small Sternis
    ul
      .tb-entry(v-for="v,k in animaldata.insekten" v-if="search.length==0 | v.Name.toLowerCase().indexOf(search.toLowerCase())!==-1")
        .typ Insekt
        .name {{v.Name}}
        .price 
          span {{v.Verkaufspreis}}
          span.small Sternis
</template>

<script>
import * as data from '../data.json';


module.exports = {

  data: function () {
    return {
      search: "",
      animaldata: data
    }
  }
}
</script>

<style scoped>
.tb-entry {
  display:flex;
  flex-direction: row;
  width:100vw;
  font-size:4vw;
}
.tb-entry  > * {
  flex:3;
}
.tb-entry  > .typ {
  flex:1;
}
.tb-entry  > .price {
  flex:1;
}
.fw-input {
  width:95vw;
  display:block;
  font-size:4vw;border:2px black solid;
  margin:auto;
}
comphead {
  width:100vw;
}
span.small {
  font-size:2vw;
}
</style>