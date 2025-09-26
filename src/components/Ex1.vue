<script>
    export default { 
 
        data() {
            return {
                message: "Choose your favourite fruit:",
                fruit1: "Apple",
                fruit2: "Orange",
                fruit3: "Peach",
                fruits: ["Apple", "Orange", "Peach"]
            }
        }
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
    </div>
    <h3> Using Array</h3>
    {{message}}</br>
    <span v-for="fruit in fruits">
        {{fruit}}<input type="radio" name="fruit">
    </span>
</template>

<style scoped>
</style>
