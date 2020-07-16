<script>
    import { Router, Route } from "svelte-routing";

    import Editor from "./routes/Editor.svelte";
</script>

<main>
    <Router>
        <Route path="/" component={Editor} />
    </Router>
</main>
