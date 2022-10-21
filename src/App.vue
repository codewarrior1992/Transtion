<script setup>
import { ref } from "vue";
import TransitionDemo from "./components/TransitionDemo.vue";
const toggle = ref(false);
</script>
<template>
  <section>
    <button
      type="button"
      class="container buttonOne"
      @click="toggle = !toggle"
      :class="{ active: toggle }"
    >
      <div class="top">我是標題</div>
      <div class="bottom">
        <div class="content">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat
          animi ea quod quos perferendis, odio commodi, dolorem amet dignissimos
          dicta suscipit? Fugit, explicabo eius autem libero perferendis dolorem
          eos deleniti.
        </div>
      </div>
    </button>

    <TransitionDemo />
  </section>
</template>
