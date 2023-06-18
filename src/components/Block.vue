<template>
    <div class="block" v-if="showBlock">
        click me
    </div>
</template>

<script>

    export default {
        props: ["delay"],
        data() {
            return {

                showBlock: false
            }
        },
        mounted() {
            console.log("showBlock")
            setTimeout( () => {this.showBlock = true, console.log(this.delay)}, this.delay)
        } ,
        updated() {

        }
    }

</script>

<style>

.block {
    width: 400px;
    border-radius: 20px;
    background: #444;
    color: #fff;
    text-align: center;
    padding: 100px 0;
    margin: 40px auto;
}

</style>