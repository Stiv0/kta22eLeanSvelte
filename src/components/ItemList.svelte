<script>
    export let items,title;
</script>
<div class="content">
    <h1>{title}</h1>
    <ul>
        {#each items as item}
        <li>{item.name}
        <input type="checkbox" bind:checked={item.done}>
        </li>
        {/each}
    </ul>
</div>