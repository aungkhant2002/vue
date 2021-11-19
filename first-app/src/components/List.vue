<template>
    <li class="list-group-item" @dblclick="isEdit=true">
        <input v-if="isEdit" type="text" class="form-control" v-model="listText" @keyup.enter="isEdit=false">
        <span v-else>{{ listText }}</span>
    </li>
</template>

<script>
export default {
    name: "List",
    data() {
        return {
            listText: "",
            isEdit: true,
        }
    },
}
</script>

<style scoped>

</style>