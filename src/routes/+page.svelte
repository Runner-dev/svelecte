<script>
  import Svelecte from '$lib/Svelecte.svelte';

  const items = 10;
  let options = [];
  for (let i = 1; i <= items; i++) {
    options.push({id: i, text: `Item #${i}`});
  }
</script>

<div class="container">
  <Svelecte {options} multiple value={[3,7]} clearable />
</div>

<style>
  .container {
    width: 492px;
    margin: 2rem auto;
  }
</style>