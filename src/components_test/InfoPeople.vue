<template>
    <div>
        <p v-if="its_work">I am work in moment</p>
        <p v-else="its_work">I not work in moment</p>
        <p>Techs:</p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
        </ul>
        <p v-show="show_email">Send message for {{ email }}</p>
        <p>Acess my website in <a v-bind:href="website">click here!</a></p>

        <Picture />
    </div>
</template>

<script>
    import Picture from "./Picture.vue";    
    export default {
        name: "Info",
        components: {
            Picture,
        },  
        data(){
            return {
                its_work: true,
                show_email: true,
                email:"anderson@gmail.com",
                website: "https://google.com",
            }
        }
        }
</script>