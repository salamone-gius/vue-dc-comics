<template>
    <main>
        <JumboTron/>
        <ComicsSection/>
    </main>
</template>

<script>
import JumboTron from './JumboTron.vue'
import ComicsSection from './ComicsSection.vue'

export default {
    name: 'BaseMain',
    components: {
        JumboTron,
        ComicsSection,
    }
}
</script>

<style lang='scss' scoped>

main {
    background-color: var(--quaternary-color);
    color: var(--primary-color);
    font-size: 1.5rem;
}

</style>