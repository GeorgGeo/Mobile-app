<template>
    <nav class="navbar navbar-dark bg-success">
    <div class="container-fluid">
        <a href="#" class="navbar-brand">Marvel</a>
        <form class="d-flex">
            <input type="search"
                   placeholder="Поиск..."
                   aria-label="Search"
                   class="form-control me-2"
                   v-model.trim="search"
                   @input="changeSearch(search)"
            >
            <button
                    type="reset"
                    class="btn btn-outline-light"
            >
                все
            </button>
        </form>
    </div>
</nav>
</template>

<script>
    export default {
        name: "AppHeader",
        props: ['changeSearch'],
        data() {
            return {
                search: '',
            }
        },
    }
</script>

<style scoped>

</style>
