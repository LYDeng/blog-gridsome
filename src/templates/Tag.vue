<!--
 * @Date: 2021-10-11 09:38:09
 * @LastEditors: lyd
 * @LastEditTime: 2021-10-11 16:20:15
 * @Description: 无
-->
<template>
  <Layout>
      <!-- Page Header -->
  <header class="masthead" style="background-image:url(/img/home-bg.jpg)"
  >
    <div class="overlay"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto">
          <div class="post-heading">
            <h1># {{ $page.tags.title }}</h1>
          </div>
        </div>
      </div>
    </div>
  </header>

  <!-- Post Content -->
  <article>
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto" v-for="post in $page.tags.posts" :key="post.id">
          <g-link :to="'/post/' + post.id">
            <h2>
              {{ post.title}}
            </h2>
          </g-link>
        </div>
      </div>
    </div>
  </article>
  </Layout>
</template>
<page-query>
query($id: ID!) {
    tags:strapiTag (id: $id){
        id
        title
        posts{
          id
          title
        }
    }
}
</page-query>
<script>
export default {
  name:'TagPage',
  methods: {
  },
}
</script>

<style>

</style>