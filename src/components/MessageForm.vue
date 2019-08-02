<template>
    <form>
        <h2>{{ title }}</h2>
        <p><textarea type="text" placeholder="Your message!"></textarea></p>
        <p><button type="submit">Let's go!</button></p>
    </form>
</template>

<script lang="ts">
    import { Component, Prop, Vue } from 'vue-property-decorator';

    @Component
    export default class MessageForm extends Vue {
        @Prop() private title!: string;
    }
</script>

<!--&lt;!&ndash; Add "scoped" attribute to limit CSS to this component only &ndash;&gt;-->
<!--<style scoped lang="scss">-->
<!--    h3 {-->
<!--        margin: 40px 0 0;-->
<!--    }-->
<!--    ul {-->
<!--        list-style-type: none;-->
<!--        padding: 0;-->
<!--    }-->
<!--    li {-->
<!--        display: inline-block;-->
<!--        margin: 0 10px;-->
<!--    }-->
<!--    a {-->
<!--        color: #42b983;-->
<!--    }-->
<!--</style>-->
