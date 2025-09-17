<script lang="ts">
  import ClosedJournal from "$comp/journal/ClosedJournal.svelte";

  let { contains = '0' } = $props();
</script>

<div class="decor">
    {#if contains == '1'}
        <ClosedJournal />
    {:else}
        0
    {/if}
</div>

<style>
    .decor {
        border: 1px blue solid;
        padding: 3px;
        text-align: center;
    }
</style>