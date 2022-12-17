<script lang="ts">
  import About from "@src/components/About.svelte";
  let name = "typescript";
  let active = false;
</script>


<h1 class:active>Svelte {name} version</h1>
<button on:click={() => active = !active}>Toggle Active</button>

<About />
<style lang="scss">
  .active {
    color: red;
    &:hover{
      color:blue;
    }
  }
</style>
