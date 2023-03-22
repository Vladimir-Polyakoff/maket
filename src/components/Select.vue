<script>
export default {
  name: 'TheSelect',

  props: {
    list: { type: Array, required: true },
    selected: { type: String, required: true }
  },

  data () {
    return {
      showList: false
    }
  },

  mounted () {
    document.addEventListener('click', this.hideList)
  },
  destroyed () {
    document.addEventListener('click', this.hideList)
  },

  methods: {
    hideList () {
      this.showList = false
    }
  }
}
</script>

<template>
<div>
  <div class="select">
    <div class="title"
      @click.stop="showList = !showList"
    >{{ selected }}
  </div>
    <div class="body" v-if="showList">
      <div
        v-for="item in list"
        :key="item"
        @click="$emit('selectOption', item)"
      >{{ item }}
      </div>
    </div>
  </div>
</div>
</template>

<style scoped lang="scss">
  .select {
    width: 200px;
    border: 1px solid #ccc;
  }
  .title {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 30px;
    border-bottom: 1px solid #ccc;
    background: #ccc;
  }
  .body{
    div {
      padding: 10px;
      font-size: 20px;
      cursor: pointer;
      &:hover {
        background: #cccccc80;
      }
    }
  }
</style>
