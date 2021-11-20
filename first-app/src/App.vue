<template>
    <div class="p-3">
        <ListTitle title="This is List Title" :badge-title="12"></ListTitle>
        <ul>
            <List v-for="(fruit, index) in fruits" :key="index" :list-text="fruit" :current-index="index" @toParent="run"></List>
        </ul>
    </div>
</template>

<script>
import ListTitle from "./components/ListTitle";
import List from "./components/List";
export default {
    name: "App",
    components: {List, ListTitle},
    data() {
        return {
            fruits: ["apple", "orange", "mango", "banana"],
        }
    },
    methods: {
        run(x) {
            this.fruits.splice(x, 1);
        }
    },
}
</script>

<style scoped>

</style>