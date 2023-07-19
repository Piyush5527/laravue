<template>
    {{ listing.id }}
    {{ listing.city }}, {{ listing.street }}, {{ listing.street_number }},
    for ${{ listing.price }},
</template>
<script setup>
defineProps({
    listing: Object,
});
</script>
