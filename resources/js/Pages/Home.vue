<template>
    <h1>Welcome {{ name }}</h1>
    <ul>
        <li v-for="framework in frameworks">
            {{ framework }}
        </li>
    </ul>
    <Nav></Nav>
</template>

<script>
import Nav from '../Shared/Nav.vue';
export default {
    components: {
        Nav
    },
    props: {
        name: String,
        frameworks: Array
    }
}
</script>
