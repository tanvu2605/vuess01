<template>
  <div>
    <h2>Thông tin cá nhân</h2>
    <ul>
      <li>Họ và tên: <strong>{{ user.fullName }}</strong></li>
      <li>Giới tính: <strong>{{ user.gender }}</strong></li>
      <li>Ngày sinh: <strong>{{ user.birthDate }}</strong></li>
      <li>Email: <strong>{{ user.email }}</strong></li>
      <li>Địa chỉ: <strong>{{ user.address }}</strong></li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        fullName: 'Nguyễn Văn A',
        gender: 'Nam',
        birthDate: '06/03/2024',
        email: 'nva@gmail.com',
        address: 'Thanh Xuân, Hà Nội'
      }
    };
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
strong {
  font-weight: bold;
}
</style>
