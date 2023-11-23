<template>
    <div>
        <h2>This is description of people: {{ name }}</h2>
       <InfoPeople />
    </div>
</template>

<script>
import InfoPeople from './InfoPeople.vue';
    export default {
    name: "People - And",
    components: {
        InfoPeople,
    },
    data() {
        return {
            name: "Anderson",
        };
    },
    components: { InfoPeople }
}
</script>