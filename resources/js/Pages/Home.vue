<template>
    <Layout>
        <h1>Welcome {{ name }}</h1>
        <ul>
            <li v-for="framework in frameworks">
                {{ framework }}
            </li>
        </ul>
    </Layout>
</template>

<script>
import Layout from "../Shared/Layout";
export default {
    components: {
        Layout
    },
    props: {
        name: String,
        frameworks: Array
    }
}
</script>
