<template>
    <div>
        <header>
            <navbar-component/>
        </header>
        <main>
            <slot></slot>
        </main>
        <footer>
            <end-component></end-component>
        </footer>
    </div>
</template>
<script>
import EndComponent from '@/components/EndComponent.vue';
import NavbarComponent from '@/components/NavbarComponent.vue';
export default {
  components: { EndComponent, NavbarComponent },
    name:'TemplateView'
}
</script>
<style scoped>

</style>