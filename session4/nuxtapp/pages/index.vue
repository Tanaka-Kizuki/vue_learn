<template>
  <section class="container">
    <h1>{{title}}</h1>
    <p>{{$store.state.message}}</p>
    <hr>
    <div class="link"
     @click="$store.dispatch('doit')">
      <a>
        Clicked: {{$store.state.counter}}
      </a>
    </div>
  </section>
</template>

<script>
export default {
  data:function() {
    return {
      title:'Hello',
      message:'This is message',
    };
  },
  methods: {
    doAction:function() {
      this.$store.state.counter ++;
    }
  }
}
</script>

<style>

</style>
