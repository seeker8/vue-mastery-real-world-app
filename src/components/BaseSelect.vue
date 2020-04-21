<template>
  <div>
    <label v-if="label">{{ label }}</label>
    <select v-on="$listeners" @input="updateValue" v-bind="$attrs">
      <option
        v-for="option in options"
        :key="option"
        :value="value"
        :selected="option === value"
        >{{ option }}</option
      >
    </select>
  </div>
</template>

<script>
import { formFieldMixin } from '@/mixins/formFieldMixin.js'

export default {
  mixins: [formFieldMixin],
  props: {
    options: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped></style>
