<template>
    <!-- dfds -->
    <div v-if="$page.props.flash.message" class="success">
        {{ $page.props.flash.message }} AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
        Message.
    </div>
    <!-- <div>{{ flashSuccess }} lll </div> -->
    <div v-for="listing in listings" :key="listing.id">
        <Link :href="`/listing/${listing.id}`">
            <ListingAddress :listing="listing"/>
        </Link>
    </div>
</template>
<script setup>
import { Link,usePage } from "@inertiajs/vue3";
import ListingAddress from "../../Components/ListingAddress.vue";
import { computed } from "@vue/reactivity";
// const page = usePage()
// const flashSuccess = computed( () => usePage().props.flash.message, )
defineProps({
    listings: Array,
});
</script>
<style scoped>
    .success{
        text-color:green;
        background-color: white;
    }
</style>
