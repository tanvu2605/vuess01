<template>
  <div class="container">
    <div class="box" :style="{ backgroundColor: color }">
      Box
    </div>
    <div class="label">
      {{ color }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'ColorBox',
  props: {
    color: {
      type: String,
      required: true,
      validator: function (value) {
        // Chỉ chấp nhận các màu: red, blue, green
        return ['red', 'blue', 'green'].includes(value);
      }
    }
  }
};
</script>

<style scoped>
.container {
  display: inline-block;
  text-align: center;
  margin: 0 20px;
}

.box {
  width: 200px;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-weight: bold;
  font-size: 20px;
}

.label {
  margin-top: 10px;
  padding: 5px 10px;
  border: 1px solid #ccc;
  display: inline-block;
  font-size: 16px;
  text-transform: lowercase;
}
</style>
