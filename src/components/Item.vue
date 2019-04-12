<template>
  <div>
    <i @click="checked=!checked" v-if="checked" class="material-icons">check_box</i>
    <i @click="checked=!checked" v-if="!checked" class="material-icons">check_box_outline_blank</i>
    <span>{{text}}</span>
  </div>
</template>

<script>
  export default {
    name: "Item",
    data: () => ({
      checked: false
    }),
    props: {
      text: String
    }
  }
</script>

<style>
i {
  vertical-align: middle;
  cursor: pointer;
}
</style>
