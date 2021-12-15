<template>
    <li>
        {{label}}
        <i class="fas fa-chevron-down" v-if="children? 'true':''" ></i>
        <ul class="submenu">
            <li v-for="(item, i) in children" :key="i">
                {{item.label}}
            </li>
        </ul>
    </li>
</template>
<script>

export default {
  props: {
     label: String,
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
        font-size: .9em;
        &:hover {
            background-color: #eee;
            .submenu {
                display: block;
            }
        }
        i {
            font-size: 10px;
        }
        ul {
            &.submenu {
                display: none;
                position: absolute;
                left: 0;
                right:0;
                top: 80px;
                background-color: white;

                li {
                    display: block;
                    line-height: 40px;
                    margin: 0;
                }
            }
        }
    }
</style>