<template>
    <Head>
        <title>My App</title>
        <meta type="Wdescription" content="Information about my app" head-key="description">
    </Head>
    <section class="p-6 bg-gray-100">
        <header class="flex justify-between">
            <div class="flex items-center">
                <h1 class="font-bold text-lg">My App</h1>

                <!-- <p class="text-sm ml-4">Welcome back, {{ username }}</p> -->
            </div>

            <Nav />
        </header>
    </section>

    <section class="p-6">
        <div class="max-w-3xl mx-auto">
            <slot />
        </div>
    </section>
</template>

<script>
    import Nav from "./Nav";

    export default {
        components: { Nav },
        computed: {
            // username() {
            //     return this.$page.props.auth.user.username
            // }
        }
    };
</script>

