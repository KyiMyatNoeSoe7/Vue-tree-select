<template>
  <div id="app">
    <HelloWorld msg="Tree Select"/>
    <TreeSelect v-model="value" :multiple="true" :options="options" :disable-branch-nodes="true"
  :show-count="true"
  placeholder="Select ...." @search-change="searchChange"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

import TreeSelect from '@riophae/vue-treeselect'
import '@riophae/vue-treeselect/dist/vue-treeselect.css'

export default {
  name: 'App',
  components: {
    HelloWorld,
    TreeSelect
  },
  data() {
      return {
        // define the default value
        value: null,
        options: [ {"id":"1","label":"A","children": [ {"id": "24","label": "aa",},{"id": "25","label": "aa",},{"id": "26","label": "aa",} ] },
                  {"id":"2","label":"B","children": [ {"id": "21","label": "bb",},{"id": "22","label": "bb",},{"id": "23","label": "bb",} ] },
                  {"id":"3","label":"C","children": [ {"id": "31","label": "cc",},{"id": "32","label": "cc",},{"id": "33","label": "cc",} ] },
                  {"id":"4","label":"D","children": [ {"id": "41","label": "dd",},{"id": "42","label": "dd",},{"id": "43","label": "dd",} ] },
                  {"id":"5","label":"E","children": [ {"id": "51","label": "ee",},{"id": "52","label": "ee",},{"id": "53","label": "ee",} ] },
                  {"id":"6","label":"F","children": [ {"id": "61","label": "ff",},{"id": "62","label": "ff",},{"id": "63","label": "ff",} ] },
                  {"id":"7","label":"G","children": [ {"id": "71","label": "gg",},{"id": "72","label": "gg",},{"id": "73","label": "gg",} ] },
                  {"id":"8","label":"H","children": [ {"id": "81","label": "hh",},{"id": "82","label": "hh",},{"id": "83","label": "hh",} ] },
                  {"id":"9","label":"I","children": [ {"id": "91","label": "ii",},{"id": "92","label": "ii",},{"id": "93","label": "ii",} ] },
                  {"id":"10","label":"J","children": [ {"id": "101","label": "jj",},{"id": "102","label": "jj",},{"id": "103","label": "jj",} ] },
                  {"id":"11","label":"K","children": [ {"id": "111","label": "kk",},{"id": "112","label": "kk",},{"id": "113","label": "kk",} ] },
                  {"id":"12","label":"M","children": [ {"id": "121","label": "mm",},{"id": "122","label": "mm",},{"id": "123","label": "mm",} ] },
                  {"id":"13","label":"N","children": [ {"id": "131","label": "nn",},{"id": "132","label": "nn",},{"id": "133","label": "nn",} ] },
                  {"id":"14","label":"O","children": [ {"id": "141","label": "oo",},{"id": "142","label": "oo",},{"id": "143","label": "oo",} ] },
                  {"id":"15","label":"P","children": [ {"id": "151","label": "pp",},{"id": "152","label": "pp",},{"id": "153","label": "pp",} ] },
                  {"id":"16","label":"Q","children": [ {"id": "161","label": "qq",},{"id": "162","label": "qq",},{"id": "163","label": "qq",} ] },
                  {"id":"17","label":"R","children": [ {"id": "171","label": "rr",},{"id": "172","label": "rr",},{"id": "173","label": "rr",} ] },
                  {"id":"18","label":"S","children": [ {"id": "181","label": "ss",},{"id": "182","label": "ss",},{"id": "183","label": "ss",} ] },
                  {"id":"19","label":"T","children": [ {"id": "191","label": "tt",},{"id": "192","label": "tt",},{"id": "193","label": "tt",} ] },
                  {"id":"20","label":"U","children": [ {"id": "201","label": "uu",},{"id": "202","label": "uu",},{"id": "203","label": "uu",} ] },
                  
                ],
      }
  },
   methods: {
            searchChange () {
                // console.log(target.value);    
            }
   },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
