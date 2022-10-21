<script setup>
import { ref } from "vue";
const toggle = ref(false);
</script>
<template>
  <section>
    <button type="button" class="container buttonTwo" @click="toggle = !toggle">
      <div class="top">我是標題</div>
      <Transition name="slide">
        <div class="bottom" v-if="toggle">
          <div class="content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat
            animi ea quod quos perferendis, odio commodi, dolorem amet
            dignissimos dicta suscipit? Fugit, explicabo eius autem libero
            perferendis dolorem eos deleniti.
          </div>
        </div>
      </Transition>
    </button>
  </section>
</template>
