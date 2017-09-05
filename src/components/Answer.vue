<template>
    <div class="alert alert-success text-center" >
        <h1 style="color:#fff">That's Correct!</h1>
    <br>
        <button class="btn btn-warning" @click="onNextQuestion">Next Question</button>
    </div>
</template>
<style>

</style>
<script>

    export default{
        methods: {
            onNextQuestion() {
                this.$emit('confirmed');
            }
        }
    }
</script>
