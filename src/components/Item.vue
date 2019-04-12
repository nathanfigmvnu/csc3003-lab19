<template>
  <div>
    <i @click="checked=!checked" v-if="checked" class="material-icons">check_box</i>
    <i @click="checked=!checked" v-if="!checked" class="material-icons">check_box_outline_blank</i>
  </div>
</template>

<script>
  export default {
    name: "Item",
    data: () => ({
      checked: false
    })
  }
</script>

<style>
i {
  vertical-align: middle;
  cursor: pointer;
}
</style>
