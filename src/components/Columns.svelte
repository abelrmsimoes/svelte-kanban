<script>
  import Column from './Column.svelte';
  import { store } from '../stores/store';
</script>

<div>
  {#each $store as column, idx (column.id)}
    <section id={column.id} {idx}>
      <Column {column} {idx} />
    </section>
  {/each}
</div>
