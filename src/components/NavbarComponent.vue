<template>
  <div class="center examplex">
    <vs-navbar color="dark" text-white square center-collapsed v-model="active" class="custom-navbar">
      <template #left>
        <img src="assets/l.png" alt="Do-IT">
      </template>
      <vs-navbar-item :active="active == 'home'" id="home" class="nav-item" @click.prevent="$router.push({ name: 'home' })">
        Home
      </vs-navbar-item>

      <vs-navbar-item :active="active == 'about'" id="about" class="nav-item" @click.prevent="$router.push({name:'about'})">
        About us
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'Courses'" id="Courses" class="nav-item" @click.prevent="$router.push({name:'courses'})">
        Courses
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'offers'" id="offers" class="nav-item" @click.prevent="$router.push({name:'offers'})">
        Offers
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'contact'" id="contact" class="nav-item" @click.prevent="$router.push({name:'contact'})">
        Contact us
      </vs-navbar-item>
      <template #right>
        <vs-button color="warn" flat >Login</vs-button>
        <vs-button color="warn" border >Sign Up</vs-button>
      </template>
    </vs-navbar>
  </div>
</template>

<script>
export default {
  name: 'NavbarComponent'
}
</script>

<style scoped>
::v-deep .custom-navbar .nav-item {
  color: rgba(176, 145, 51, 0.966);
}
</style>
