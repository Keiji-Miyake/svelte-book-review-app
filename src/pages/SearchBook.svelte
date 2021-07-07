<script lang="ts">
    import SearchBar from '../components/SearchBar.svelte'

    let q = ''
</script>

<div>
    <SearchBar bind:value={q} />
</div>

<div class="text-center mt-4">
    { q }
</div>