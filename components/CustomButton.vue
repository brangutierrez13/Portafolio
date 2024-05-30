<template>
    <a :href="link" @click="$emit('action')" :class="customClass + ' flex flex-row items-center justify-center cursor-pointer'">
        <i :class="icon"></i>
        <div class="ml-2">{{ text }}</div>
    </a>
</template>

<script>
export default {
    props: {
        text: String,
        icon: String,
        link: String,
        customClass: String,
    }
}
</script>