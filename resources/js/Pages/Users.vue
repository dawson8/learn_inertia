<template>
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
</template>


<script>
    import Layout from "../Shared/Layout";
    import { Link } from "@inertiajs/inertia-vue3";

    export default {
        layout: Layout,
        props: { time: String }
    };
</script>

