<script>
    import Navbar from "$lib/components/Navbar.svelte";
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Footer from "$lib/components/Footer.svelte";
</script>

<Navbar />
<ModeWatcher />

<main class="min-h-[calc(100vh-10.5rem)]">
    <slot />
</main>

<Footer />