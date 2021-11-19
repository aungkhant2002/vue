<template>
    <div class="p-3">
        <Title></Title>
        <ul class="list-group">
            <List></List>
            <List></List>
            <List></List>
            <List></List>
        </ul>
    </div>
</template>

<script>
import Title from "./components/Title";
import List from "./components/List";
export default {
    name: "App",
    components: {List, Title},
}
</script>

<style scoped>

</style>