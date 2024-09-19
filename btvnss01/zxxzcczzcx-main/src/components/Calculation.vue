<template>
  <div>
    <h2>Danh sách kết quả</h2>
    <ul>
      <li>{{ a }} + {{ b }} = {{ add(a, b) }}</li>
      <li>{{ a }} - {{ b }} = {{ subtract(a, b) }}</li>
      <li>{{ a }} * {{ b }} = {{ multiply(a, b) }}</li>
      <li>{{ a }} / {{ b }} = {{ divide(a, b) }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      a: 10,
      b: 10
    };
  },
  methods: {
    add(a, b) {
      return a + b;
    },
    subtract(a, b) {
      return a - b;
    },
    multiply(a, b) {
      return a * b;
    },
    divide(a, b) {
      return b !== 0 ? a / b : 'Cannot divide by zero';
    }
  }
};
</script>

<style scoped>
h2 {
  font-family: Arial, sans-serif;
  font-weight: bold;
}
ul {
  list-style-type: disc;
}
</style>
