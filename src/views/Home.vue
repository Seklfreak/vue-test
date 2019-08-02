<template>
  <div class="home">
    <h1>Wow!</h1>
    <p>I am a Vue.js dev now!</p>
    <MessageForm title="Fill this out pls"></MessageForm>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import MessageForm from '@/components/MessageForm.vue'; // @ is an alias to /src

@Component({
  components: {
    MessageForm,
  },
})
export default class Home extends Vue {}
</script>
