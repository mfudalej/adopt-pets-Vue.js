<template>
  <div>
    <PetTable
      species="dogs"
      :pets="dogs"
    />
  </div>
</template>

<script>
  import { mapState } from "vuex"
  import PetTable from '@/components/PetTable.vue'
  
  export default {
    name: 'Dogs.vue',
    components: {
      PetTable
    },
    data () {
      return {}
    },
    computed: {
      ...mapState([
        'dogs'
      ])
    }
  }
</script>

<style scoped>

</style>
