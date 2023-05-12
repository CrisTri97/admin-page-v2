<template>
  <div class="center">
    <vs-select v-model="value8" :label-placeholder="placeholder">
      <vs-option
        v-for="item of values"
        :key="item.label"
        :label="item.label"
        :value="item.id"
      >
        {{ item.value }}
      </vs-option>
    </vs-select>
  </div>
</template>

<script>
export default {
  name: 'SelectComponent',
  props: {
    values: {
      type: Array,
      required: true,
      default: () => {}
    },
    placeholder: {
      type: String,
      required: true,
    },
  },

  data: () => ({
    value8: '',
  }),
}
</script>
