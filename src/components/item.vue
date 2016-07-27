<template>
  <div class="item">
    <span class="list">{{index}}.</span>
    <p>
      <a class="title" :href="href" target="_blank">{{{item.title}}}</a>
      <span class="lj" v-show="showDomain">
        ({{item.url | domain}})
      </span>
    </p>
  </div>
</template>

<script>
export default {
  name: 'Item',
  props: {
    item: Object,
    index: Number
  },
  computed: {
    href (){
      return this.item.url || ('#/item/'+this.item.id)
    },
    showDomain () {
      return this.item.type === 'story'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
