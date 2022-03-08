<template></template>

<script lang="ts">
import { defineComponent } from "vue";
import axios from "../utils/axios";

export default defineComponent({
    setup() {
        axios.get('/user/nicollin').then((res) => {
            console.log('res:', res);
        }).catch(err => {
            console.log('err:', err);
        })
    }
})

</script>

<style scoped>
</style>