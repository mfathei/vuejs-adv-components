<template>
<div>
    <button @click="counter++">Increase</button>
    <p>{{ counter }}</p>
</div>  
</template>

<script>
export default {
  data() {
    return {
      counter: 0
    };
  },
  destroyed() {
    console.log("Destroyed!");
  },
  activated() {
    console.log("activated!");
  },
  deactivated() {
    console.log("deactivated!");
  }
};
</script>

