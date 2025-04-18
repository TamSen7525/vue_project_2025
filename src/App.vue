<template>
  <div>
    <User :arg="[1, 2, 3, 4, 5]" />
  </div>
</template>

<script>
import User from './components/User.vue'

export default {
  components: {
    User
  }
};
</script>