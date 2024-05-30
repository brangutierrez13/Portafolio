<template>
    <div class="flex flex-row flex-wrap gap-5">
        <div v-for="(item, i) in SocialLinks" :key="i" class="text-4xl cursor-pointer">
            <NuxtLink :to="item.route">
                <i :class="item.icon"></i>
            </NuxtLink>
        </div>
    </div>
</template>

<script>
export default{
    data: () => ({
        SocialLinks: [
            {
                name: 'facebook', route: '', icon: 'bi bi-facebook',
            },
            {
                name: 'Instagram', route: '', icon: 'bi bi-instagram',
            },
            {
                name: 'GitHub', route: '', icon: 'bi bi-github',
            },
            {
                name: 'Linkedin', route: '', icon: 'bi bi-linkedin',
            }
        ]
    }),
}
</script>