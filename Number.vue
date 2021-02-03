<template>
    <div>
        <h1>{{result}}</h1>
        <form v-on:submit= "onSubmitForm">
            <input type="text" ref="answer" v-model="value">
            <button>hi!</button>
        </form>
        <div> 시도:{{}}</div>
    </div>
    
</template>

<script>
export default {
    data() {
        return {
            value: "",
            result: "",
        }
    },
    methods: {
        onSubmitForm(e) {
            e.preventDefault();
        }
    }
};
</script>

<style>

</style>