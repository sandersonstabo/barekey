<script>
    import * as Item from "$lib/components/ui/item";
    import clsx from "clsx";
    import { mode } from "mode-watcher";

    const bg_gradient = mode.current === "dark" 
    ? "bg-gradient-to-b from-background to-sky-700"
    : "bg-gradient-to-b from-background to-sky-700";
</script>

<div class="w-screen h-screen {bg_gradient}">

</div>