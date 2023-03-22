
<template>
  <input
    type="number"
    :value="value"
    @input="$event => $emit('input', Number($event.target.value.trim()))"
  >
</template>

<script>
export default {
  name: 'TheFied',

  props: {
    value: { type: [Number, String], required: true }
  }
}
</script>
