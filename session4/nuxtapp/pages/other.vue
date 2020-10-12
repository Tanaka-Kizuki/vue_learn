<template>
     <section class="container">
          <h1>{{title}}</h1>
          <p>{{message}}</p>
          <hr>
          <pre>{{now}}</pre>
          <router-link to="/">Go to top</router-link>
     </section>
</template>

<script>
export default {
     data:function() {
          return {
               title: 'Other',
               message: 'これは、別のページです',
          }
     }
}
</script>