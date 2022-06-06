<template>
    <main>
        <div>
            <JumboTron/>            
        </div>
    </main>
</template>

<script>
import JumboTron from './JumboTron.vue'
export default {
    name: 'BaseMain',
    components: {
        JumboTron,
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