<template>
    <div class="p-3">
        <ListTitle title="This is List Title" :badge-title="12"></ListTitle>
        <ul>
            <List list-text="apple"></List>
            <List list-text="orange"></List>
            <List list-text="mango"></List>
            <List list-text="lemon"></List>
        </ul>
    </div>
</template>

<script>
import ListTitle from "./components/ListTitle";
import List from "./components/List";
export default {
    name: "App",
    components: {List, ListTitle},
}
</script>

<style scoped>

</style>