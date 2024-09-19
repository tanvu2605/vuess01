<template>
  <div>
    <h2>Họ và tên: <strong>{{ formatName(user) }}</strong></h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        firstName: 'Nguyễn Văn',
        lastName: 'Nam'
      }
    };
  },
  methods: {
    formatName(user) {
      return `${user.firstName} ${user.lastName}`;
    }
  }
};
</script>

<style scoped>
h2 {
  font-family: Arial, sans-serif;
  font-weight: bold;
}
strong {
  font-weight: bold;
}
</style>
