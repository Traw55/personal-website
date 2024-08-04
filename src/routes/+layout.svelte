<script>
    import Navbar from "$lib/components/Navbar.svelte";
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
</script>

<Navbar />
<ModeWatcher />
<slot></slot>
