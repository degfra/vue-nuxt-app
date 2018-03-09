<!-- nuxt-child in a /pages/file.vue : 
     will display the content of any sub routes of the /pages/users folder :
     => more generally, any subroute of the /pages/<subfolder>
     whose name == the file name of the .vue file where nuxt-child resides -->

<template>
    <div>
        <input type="text" v-model="userId">
        <button @click="onLoadUser">Load User</button>
        <nuxt-child />
    </div>
</template>

<script>
export default {
  data() {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId)
    }
  },
  layout: 'users'
}
</script>
