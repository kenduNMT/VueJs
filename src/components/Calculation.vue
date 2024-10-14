<template>
    <div class="calculator">
        <h2>Máy Tính</h2>
        <input v-model="num1" type="number" placeholder="Nhập số đầu" />
        <input v-model="num2" type="number" placeholder="Nhập số sau" />
        <div class="results">
            <h3>Danh sách kết quả</h3>
            <li>Phép cộng: {{ add() }}</li>
            <li>Phép trừ: {{ subtract() }}</li>
            <li>Phép nhân: {{ multiply() }}</li>
            <li>Phép chia: {{ divide() }}</li>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

// Khai báo các biến để lưu trữ giá trị nhập vào
const num1 = ref(0)
const num2 = ref(0)

// Hàm cộng
const add = () => {
    return num1.value + num2.value
}

// Hàm trừ
const subtract = () => {
    return num1.value - num2.value
}

// Hàm nhân
const multiply = () => {
    return num1.value * num2.value
}

// Hàm chia
const divide = () => {
    if (num2.value === 0) {
        return 'Cannot divide by zero'
    }
    return num1.value / num2.value
}
</script>

<style scoped>
.calculator {
    max-width: 300px;
    margin: auto;
    text-align: center;
}

input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}

.results {
    margin-top: 20px;
    text-align: left;
}
</style>