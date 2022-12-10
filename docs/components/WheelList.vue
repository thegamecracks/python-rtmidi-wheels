<script setup>
const wheelData = await fetch(
    "https://api.github.com/repos/thegamecracks/python-rtmidi-wheels/contents/dist",
    {
        headers: {
            Accept: "application/vnd.github+json",
        },
    },
).then((response) => response.json())
</script>

<template>
    <h1>Wheels for sale!</h1>
    <ul class="no-dots">
        <li v-for="wheel in wheelData" :key="wheel.name">
            <a :href="wheel.download_url">
                {{ wheel.name }}
            </a>
        </li>
    </ul>
</template>

<style>
.no-dots {
    list-style-type: none;
}
</style>
