<script setup>
import { ref } from 'vue';
const bøger = ref([
    {
        titel: "To kill a mockingbird",
        forfatter: "Harper Lee"
    },
    {
        titel: "The seven husbands of Evelyn Hugo",
        forfatter: "Taylor Jenkins Reid"
    },
    {
        titel: "The fault in our stars",
        forfatter: "John Green"
    },
    {
        titel: "The book thief",
        forfatter: "Markus zusak"
    },
    {
        titel: "The hunger games",
        forfatter: "Suzanne Collins"
    }
]);
</script>


<template>
    <ul>
        <li v-for="i in bøger" :key="i.titel">
            Titel: {{ i.titel }}
            Forfatter: {{ i.forfatter }}
        </li>
    </ul>
</template>