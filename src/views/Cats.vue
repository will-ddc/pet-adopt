<template>
  <div class="cat-container">
    <PetTable
    species="Cats"
    :pets="cats"
    />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import PetTable from '@/components/PetTable.vue'

export default {
  name: 'cats',
  components: {
    PetTable
  },
  data () {
    return {}
  },
  computed: {
    ...mapState([
      'cats'
    ])
  }
}
</script>

<style lang="css" scoped>
</style>
