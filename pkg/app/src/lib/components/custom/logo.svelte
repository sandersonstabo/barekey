<script>
    import { theme } from "mode-watcher";

    import barekey_light from "$lib/assets/barekey-light.png";
    import barekey_dark from "$lib/assets/barekey-dark.png";

</script>
{#if theme.current == "light"}
    <img src={barekey_dark} alt="Barekey" class="h-10">
{:else}
    <img src={barekey_light} alt="Barekey" class="h-10">
{/if}