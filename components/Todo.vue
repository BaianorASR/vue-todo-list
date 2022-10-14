<template>
  <div>{{ todo }}</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { ITodo } from '@/interfaces/todo.interface';

export default defineComponent({
  name: 'Todo',
  props: {
    todo: {
      type: Object as () => ITodo,
      required: true,
    },
  },
});
</script>

<style scoped></style>
