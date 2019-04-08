<template>
    <div class="container">
        <div class="columns">
            <div class="column is-4 is-multiline">
                <div class="title is-2"
                     v-for="post in posts"
                     v-bind:key="post.id"
                     v-bind:title="post.title">{{ post.title }}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    // import Product from './Product.vue';

    export default {
        name: 'app',
        components: {
            // Product,

        },
          date:{
              posts: [
                  {id: 1, title: 'My journey with Vue'},
                  {id: 2, title: 'Blogging with Vue'},
                  {id: 3, title: 'Why Vue is so fun'}
              ],
          }
    }
</script>
<style lang="scss">
    @import "assets/global";
    @import "~bulma/bulma.sass";

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>



