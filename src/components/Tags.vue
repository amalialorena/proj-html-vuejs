<template>
  <div class="tags">
    <div class="tag" v-for="(tag, i) in tags" :key="i">
      <a :href="tag.url">{{tag.name}}</a>
    </div>
  </div>
</template>
<script>
export default {
  name: "componentName",
  props: {
    tags: [
      {
        name: String,
        url: String,
      },
    ],
  },
};
</script>

<style scoped lang='scss'>
.tags {
    display: flex;
    flex-wrap: wrap;
    .tag {
        margin-right: 5px;
        margin-bottom: 5px;
        font-size: .8em;

        &:hover {
            a {
                background-color: white;
                color: black;
            }
        }
        a {
            display: inline-block;
            border: 1px solid #444;
            padding: 5px 10px;
            color: white;
            text-decoration: none;
        }
    }
}
</style>