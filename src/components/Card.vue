<template>
    <div class="card">
        <div class="image-placeholder">
            Image
        </div>
        <div class="card-body">
            <h3>Title</h3>
            <button class="add-button">Add to card</button>
        </div>
    </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.card {
    width: 250px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    overflow: hidden;
    background-color: #fff;
    text-align: center;
    font-family: Arial, sans-serif;
}

.image-placeholder {
    width: 100%;
    height: 150px;
    background-color: #9a9a9a4b;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #000000;
    font-size: 18px;
}

.card-body {
    padding: 20px;
}

.add-button {
    padding: 10px 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #c5c5c5b8;
    cursor: pointer;
    color: #000000;
}

.add-button:hover {
    background-color: #e0e0e0;
}
</style>