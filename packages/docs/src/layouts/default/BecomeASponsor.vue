<template>
  <div
    v-if="sponsors.length > 0"
    class="pt-2 pb-2 px-2"
  >
    <app-caption
      class="ml-2 mb-1"
      path="premiere-sponsors"
    />

    <sponsor
      comfortable
      slug="teamwork"
    />

    <sponsor
      comfortable
      slug="qomplx"
    />
  </div>
</template>

<script>
  // Utilities
  import { get } from 'vuex-pathify'

  export default {
    name: 'DefaultBecomeASponsor',

    computed: { sponsors: get('sponsors/all') },
  }
</script>
