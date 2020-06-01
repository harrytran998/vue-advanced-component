<template>
  <input :value="datePicked" type="text" ref="picked" />
</template>

<script>
import Pickaday from 'pikaday'
export default {
  props: {
    datePicked: { required: true },
    format: { default: 'DD-MM-YYYY' },
    options: { default: {} },
  },
  model: {
    prop: 'datePicked',
    event: 'picked',
  },
  mounted() {
    const picker = new Pickaday({
      field: this.$refs.picked,
      format: this.format,
      onSelect: () => {
        this.$emit('picked', picker.toString())
      },
      ...this.options,
    })
  },
}
</script>

<style></style>
