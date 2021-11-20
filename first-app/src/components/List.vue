<template>
    <li>
        {{ listText }}
        <button @click="toRun()">del</button>
    </li>
</template>

<script>
export default {
    name: "List",
    props: ['listText', 'currentIndex'],
    methods: {
        toRun() {
            this.$emit("toParent", this.currentIndex);
        }
    },

}
</script>

<style scoped>

</style>