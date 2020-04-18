<template lang="pug">
html
  head
  body
    .page
      button.collapsible(type="button" v-on:click="open= !open") Wofür ist das hier?
      .content(v-if="open==true")
        h1 Das Problem.. .. und die Lösung
        br
        br
        p Ihr seid unterwegs auf einer Insel in Animal Crossing und euer Inventar ist voll? Und ihr wisst einfach nicht für was genau ihr Fische und Insekten tauschen sollt um euren Gewinn zu maximieren? Mit diesem Tool schafft ihr es effizient die Items zu tauschen um möglichst viel Geld mit nach Hause nehmen zu können!
        p Falls ihr mir einen Kaffee ausgeben wollte schickt mir gerne was zu!
        a(href="https://paypal.me/edenprjctde?locale.x=de_DE") PayPal me!
</template>

<script>
module.exports = {
 data: function () {
    return {
      open: false
    }
  }
}
</script>

<style scoped>
.collapsible {
  background-color: #eee;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.342);
}

/* Add a background color to the button if it is clicked on (add the .active class with JS), and when you move the mouse over it (hover) */
.active, .collapsible:hover {
  background-color: #ccc;
}

/* Style the collapsible content. Note: hidden by default */
.content {
  padding: 0 18px;
  overflow: hidden;
  background-color: #f1f1f1;
  
}
p{
  font-size:1em;
}
</style>