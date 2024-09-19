<template>
  <div class="card">
    <div class="card-image">
      Image
    </div>
    <div class="card-title">
      Title
    </div>
    <button class="card-button">
      Add to card
    </button>
  </div>
</template>

<script>
export default {
  name: 'Card'
};
</script>

<style scoped>
.card {
  width: 200px;
  border: 1px solid #ddd;
  border-radius: 10px;
  overflow: hidden;
  text-align: center;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}

.card-image {
  background-color: #888;
  color: white;
  padding: 40px 0;
  font-size: 20px;
}

.card-title {
  padding: 20px 0;
  font-size: 18px;
  font-weight: bold;
  border-top: 1px solid #ddd;
}

.card-button {
  margin: 10px;
  padding: 10px;
  width: 80%;
  background-color: #f9f9f9;
  border: 1px solid #ccc;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

.card-button:hover {
  background-color: #eee;
}
</style>
