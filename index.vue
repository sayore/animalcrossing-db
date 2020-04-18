<template lang="pug">
  html
    head
    <link href="https://fonts.googleapis.com/css2?family=Baloo+Bhai+2:wght@500&display=swap" rel="stylesheet">
    body
      .site
        h1 Animal Crossing - Verkaufpreise!
        animals hey
</template>
<script>
import * as data from './data.json';
import * as Animals from './components/Animals.vue';

module.exports = {
  components: {
    Animals
  },
  data: function () {
    return {
      greeting: data
    }
  }
}
</script>
<style>
/*! minireset.css v0.0.6 | MIT License | github.com/jgthms/minireset.css */html,body,p,ol,ul,li,dl,dt,dd,blockquote,figure,fieldset,legend,textarea,pre,iframe,hr,h1,h2,h3,h4,h5,h6{margin:0;padding:0}h1,h2,h3,h4,h5,h6{font-size:100%;font-weight:normal}ul{list-style:none}button,input,select,textarea{margin:0}html{box-sizing:border-box}*,*::before,*::after{box-sizing:inherit}img,video{height:auto;max-width:100%}iframe{border:0}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}td:not([align]),th:not([align]){text-align:left}
* {
  font-family: 'Baloo Bhai 2', cursive;overflow-x: hidden;
}
p {
  font-size: 2em;
  text-align: center;
}
h1 {
  text-align: center;
  font-size:3vw;
}
</style>