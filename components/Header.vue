<template>
  <header
    class="text-zinc-50 font-extrabold text-4xl bg-purple-500 h-16 flex items-center justify-center shadow"
  >
    <h1 class="cursor-pointer hover:text-zinc-100">Bai-Tod's</h1>
  </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Button } from 'flowbite-vue';

export default defineComponent({
  name: 'Header',
  components: {
    Button,
  },

  data() {
    return {
      author: 'Baianor',
      loading: false,
    };
  },

  methods: {
    setLoading() {
      this.loading = !this.loading;
    },
  },
});
</script>

<style scoped></style>
