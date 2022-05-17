<template>
    <Layout>
        <h1 class="text-3xl">Users</h1>

        <div style="margin-top: 600px">
            <p>The current time is {{ time }}.</p>

            <Link
                href="/users"
                class="text-blue-500 hover:underline"
                preserve-scroll
            >
                Refresh
            </Link>
        </div>
    </Layout>
</template>


<script>
    import Layout from "../Shared/Layout";
    import { Link } from "@inertiajs/inertia-vue3";

    export default {
        components: { Layout, Link },

        props: { time: String }
    };
</script>

