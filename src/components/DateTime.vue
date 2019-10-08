<template>
  <div
    class="text-lg"
    v-text="date"
  />
</template>

<script>
import format from 'date-fns/format';

export default {
  name: 'DateTime',
  computed: {
    date() {
      return format(new Date(), 'EEE, MMM dd hh:mm a');
    },
  },
};
</script>
