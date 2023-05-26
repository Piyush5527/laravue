<template>
    <Link href="/">main page</Link>&nbsp;&nbsp;
    <Link href="/show">show page</Link>
    <div>timer is {{ timer }}</div>

    <slot></slot>
</template>
<script setup>
    import {Link} from '@inertiajs/vue3'
    import { ref } from "vue";

    const timer = ref(0);
    setInterval(()=>timer.value++,1000)
</script>
