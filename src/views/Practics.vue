<script>
import field from '@/components/Field'
import Select from '@/components/Select'

export default {
  name: 'ThePractics',

  components: {
    field,
    Select
  },

  data () {
    return {
      first: '',
      second: '',
      third: '',
      selectList: ['+', '-', '/', '*'],
      selectedOption: ''
    }
  },

  computed: {
    // result () {
    //   return this.first && this.second && this.third ? (this.first + this.second) / this.third : ''
    // }
    result () {
      // if (this.first && this.second && this.selectedOption) {
      //   return Function(this.first + this.selectedOption + this.second)
      // }

      return ''
    }
  }
}
</script>

<template>
  <div class="practics">practics

    <field
      v-model="first"
    ></field>
    <field
      v-model="second"
    ></field>
    <!-- <field
      v-model="third"
    ></field> -->
    <div class="result" v-if="result">{{ result }}</div>
    <Select
      :list="selectList"
      :selected="selectedOption"
      @selectOption="selected => { selectedOption = selected }"
    ></Select>
  </div>
</template>

<style scoped>

  .practics {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap:10px;
    width: 200px;
    margin: 0 auto;
  }
</style>
