<template>
    <div>
        <p>Họ và tên: <strong>{{ fullName }}</strong></p>
    </div>
</template>

<script setup lang="ts">
// Khai báo đối tượng user
const user = {
    firstName: "Nguyễn Văn",
    lastName: "Nam"
}

// Hàm formatName trả về chuỗi kết hợp giữa firstName và lastName
function formatName(user: { firstName: string; lastName: string }) {
    return `${user.firstName} ${user.lastName}`;
}

// Gọi hàm formatName và lưu vào biến fullName
const fullName = formatName(user);
</script>

<style scoped>
p {
    font-size: 18px;
}

strong {
    font-weight: bold;
}
</style>