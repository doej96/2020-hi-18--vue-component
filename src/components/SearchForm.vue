<template>
  <div>
    <form>
      <SearchInput @@onChange="onChange"/>
    </form>
  </div>
</template>
<script>
import SearchInput from './SearchInput.vue'
export default {
  name: 'SearchForm',
  data() {
    return {
    }
  },
  components: {
    SearchInput
  },
  methods: {
    onChange(v) {
      this.query = v
      this.$emit('@onChange', v)
      // 또 부모에게 v(query)전달함
    }
  }
}
</script>
<style scoped>
  
</style>