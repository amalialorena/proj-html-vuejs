<template>
  <ul class="recent">
    <li v-for="(item, i) in recentPosts" :key="i">
      <a :href="item.url">{{ item.title }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "RecentPosts",
  props: {
    recentPosts: [
      {
        title: String,
        url: String,
      },
    ],
  },
};
</script>

<style scoped lang='scss'>
ul.recent {
    max-width: 100%;
    li {
        padding: 16px 0;
        border-bottom: 1px solid #444;

        display: block;
        a {
            display: block;
            color: inherit;
            text-decoration: none;
            text-overflow: ellipsis;
            overflow: hidden;
            white-space: nowrap; 
        }
    }
}
</style>