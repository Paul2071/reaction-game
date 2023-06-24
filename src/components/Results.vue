<template>
        <div>
    <p> Reaction time - {{propScore}}ms </p>
    <p class="rank">{{ rank }} </p>
</div>

</template>

<script>

    export default {
        props: ["propScore"],
        data() {
            return {
                rank: null
            }
        },
        mounted() {
            if (this.score < 250) {
                this.rank = "fastest"
            } else if (this.score < 400 ) {
                this.rank = "fast"
            } else {
                this.rank = "kinda fast"
            }
        }
    }

</script>

<style>

.rank {
    font-size: 1.4em;
    color: #444;
    font-weight: bold;
}

</style>
