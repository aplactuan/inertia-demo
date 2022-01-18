<template>
    <h2>This is the users page</h2>
    <Nav />
    <div style="margin-top: 400px">
        <p>The current time is {{ time }}</p>
        <Link href="/users" preserve-scroll>Refresh</Link>
    </div>
</template>

<script>
import Nav from "../Shared/Nav.vue";
import { Link } from '@inertiajs/inertia-vue3'
export default {
    components: {
        Nav, Link
    },
    props: {
        time: String
    }
}
</script>
