<template>
    <!-- <MainLayout> -->
        <div>jkdsjfdsjhkjk</div>
        <Link href="/show">show </Link>
        <div>{{ message }}</div>
    <!-- </MainLayout> -->
</template>

<script setup>
    import { Link } from "@inertiajs/vue3";
    import MainLayout from "../../layouts/MainLayout.vue";
    defineProps({ message: String });
</script>
<script>
    import MainLayout from "../../layouts/MainLayout.vue";
    export default {
        layout: MainLayout,
    };
</script>
