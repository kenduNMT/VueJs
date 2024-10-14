<template>
    <div class="user-info">
        <h2>Thông tin cá nhân</h2>
        <ul>
            <li>Họ và tên: <strong>{{ user.name }}</strong></li>
            <li>Giới tính: <strong>{{ user.gender }}</strong></li>
            <li>Ngày sinh: <strong>{{ user.birthdate }}</strong></li>
            <li>Email: <strong>{{ user.email }}</strong></li>
            <li>Địa chỉ: <strong>{{ user.address }}</strong></li>
        </ul>
    </div>
</template>

<script setup lang="ts">
const user = {
    name: "Nguyễn Văn A",
    gender: "Nam",
    birthdate: "06/03/2024",
    email: "nva@gmail.com",
    address: "Thanh Xuân, Hà Nội"
}
</script>

<style scoped>
.user-info {
    max-width: 300px;
    margin: auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
    background-color: #f9f9f9;
    text-align: left;
}

.user-info h2 {
    text-align: center;
    margin-bottom: 20px;
}

.user-info ul {
    list-style-type: none;
    padding: 0;
}

.user-info li {
    margin: 10px 0;
}

.user-info strong {
    font-weight: bold;
}
</style>