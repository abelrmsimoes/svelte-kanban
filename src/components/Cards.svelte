<script>
  import { store } from '../stores/store';
  import Card from './Card.svelte';

  export let column;
  export let colIdx;
</script>

<article {colIdx}>
  {#each column.cards as card, cardIdx (card.id)}
    <section class="card">
      <Card {colIdx} {card} {cardIdx} />
    </section>
  {/each}
</article>
