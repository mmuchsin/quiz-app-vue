<script setup>
import { defineProps } from 'vue';
const props = defineProps(['name', 'image', 'questions'])

</script>

<template>
    <div class="card">
        <img :src="image" alt="">
        <div class="card-text">
            <h2>{{ name }}</h2>
            <p>{{ questions }} questions</p>
        </div>
    </div>
</template>

<style>
.card {
    width: 310px;
    overflow: hidden;
    border-radius: 2%;
    box-shadow: 1px 1px 10px rgba(0, 0, 0, 0.1);
    margin-bottom: 35px;
    margin-right: 20px;
    cursor: pointer;
}

.card img {
    width: 100%;
    height: 190px;
    margin: 0
}

.card .card-text {
    padding: 0 5px
}

.card .card-text h2 {
    font-weight: bold;
}
</style>