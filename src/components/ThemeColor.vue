<template>
  <div class="theme-color">
    <color-picker
      format="hex"
      :pure-color="$store.state.mainColorBook"
      use-type="pure"
      v-model:pureColor="$store.state.mainColorBook"
      @pureColorChange="changeMainColorBook"
    />
  </div>
</template>

<script>
import { ColorPicker } from 'vue3-colorpicker';
import 'vue3-colorpicker/style.css';

export default {
  components: { ColorPicker },
  methods: {
    changeMainColorBook(newColor) {
      this.$store.commit('changeMainColorBook', newColor);
    },
  },
};
</script>

<style>
.theme-color {
  width: 128px !important;
  height: 85px !important;
  border: 2px solid #000;
}
.theme-color .vc-color-wrap.transparent {
  width: 124px !important;
  height: 81px !important;
}
</style>
