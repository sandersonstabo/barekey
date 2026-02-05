<script>
    import * as Sidebar from "$lib/components/ui/sidebar";
    import * as Item from "$lib/components/ui/item";
</script>

<div class="h-svh w-full bg-linear-to-t from-blue-950 to-sky-800 p-4">
    <Sidebar.Provider class="min-h-full h-full">
        <Sidebar.Root class="px-4 py-2 border-none">
            <Sidebar.Header>
                Hello
            </Sidebar.Header>
            <Sidebar.Content>
                content
            </Sidebar.Content>
            <Sidebar.Footer>
                Footer
            </Sidebar.Footer>
        </Sidebar.Root>

        <main class="grow">
            <Item.Root variant="muted" class="h-full">
                123
            </Item.Root>
        </main>
    </Sidebar.Provider>
</div>