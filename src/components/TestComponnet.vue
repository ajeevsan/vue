<template>
    <div>
        <div class="testClass">
            {{ message }}
        </div>

        <div class="counterDiv">{{ value }}</div>

        <button v-on:click="increment">+</button>
        <button v-on:click="decrement">-</button>
    </div>
</template>


<script>
export default {
    name: 'TestComponnet',
    props: {
        message: String
    },

    data() {
        return {
            value: 0
        };
    },

    methods: {
        increment(){
            this.value++;
        },
        decrement() {
            this.value>0?this.value--:this.value;
        }
    }
}
</script>

<style scoped="testClass">

</style>