<template>
  <li>
    <a :href="url">
      {{ label }}
      <i class="fas fa-chevron-down" v-if="children ? 'true' : ''"></i>
      <ul class="submenu" v-if="children">
        <li v-for="(item, i) in children" :key="`submenu-${i}`">
          <a :href="item.url">
            {{ item.label }}
          </a>
        </li>
      </ul>
    </a>
  </li>
</template>
<script>
export default {
  props: {
    label: String,
    url: String,
    children: Array,
  },
};
</script>
<style scoped lang="scss">
li {
  display: inline-block;
  margin-right: 20px;
  position: relative;
  cursor: pointer;
  line-height: 80px;
  height: 100%;
  font-size: 0.9em;
  padding: 0 8px;

  &:hover {
    background-color: #eee;
    .submenu {
      display: block;
    }
  }

  a {
    color: inherit;
    text-decoration: none;
    line-height: inherit;
  }

  i {
    font-size: 10px;
  }
  ul {
    &.submenu {
      display: none;
      position: absolute;
      left: 0;
      top: 80px;
      background-color: white;

      li {
        padding: 10px 16px;
        margin: 0;
        min-width: 120px;
        line-height: 1.4em;
        display: flex;
        align-items: center;
      }
    }
  }
}
</style>