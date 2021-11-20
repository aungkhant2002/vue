<template>
    <h4>
        {{ title }}
    <span class="badge badge-primary badge-pill">{{ badgeTitle }}</span>
    </h4>

</template>

<script>
export default {
    name: "ListTitle",
    props: {
        title: {
            type: String,
            required: true,
            default: "This is Default"
        },
        badgeTitle: {
            type: Number,
            required: true,
            validator(value) {
                return value>5;
            }
        }
    },
}
</script>

<style scoped>

</style>