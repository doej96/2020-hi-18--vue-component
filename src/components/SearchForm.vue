<template>
  <div>
    <form>
      <SearchInput />
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
  }
}
</script>
<style scoped>
  
</style>