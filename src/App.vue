<script setup>
import { ref } from "vue";
const count = ref(0);

const addToCount = () => {
  count.value = count.value + 1;
};

const minusFromCount = () => {
  count.value = count.value - 1;
};
</script>

<template>
  <main>
    <div>
      <h4>Our Count is ...</h4>
      <h1>
        {{ count }}
      </h1>
      <button @click="minusFromCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: rgb(223, 230, 233);
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>
