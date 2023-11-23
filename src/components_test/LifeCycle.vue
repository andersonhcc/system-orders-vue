<template>
    <h1>{{ name }}</h1>
</template>

<script>
    export default {
        name: "LyfeCycle",
        data () {
            return {
                name: "Anderson",
            }
        },
        created(){
            this.name = "Anderson LifeCycle";
        },
        mounted(){
            this.name = "Anderson mounted"
        }
    }

</script>