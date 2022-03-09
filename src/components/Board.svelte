<script>
  import { addColumn } from '../stores/store';
</script>

<section class="board">
  <button on:click={addColumn}>&plus;</button>
  <slot />
</section>
