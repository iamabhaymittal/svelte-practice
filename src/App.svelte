<script>
  import Face from "./Face.svelte";
  import Container from "./Container.svelte";
  import Header from "./Header.svelte";
  import { each } from "svelte/internal";
  import Buttons from "./Buttons.svelte";
  let say = false;
  
</script>
{#if say}
    <Header />
  
  {/if}
<Container>
  <Buttons on:click={(e) => {say = e.detail}} />

</Container>
  

<style>
  div {
    color: red;
  }
  :global(*){
    box-sizing: border-box;
  }
  :global(body,html) {
    margin: 0;
    height: 100vh;
    overflow: hidden;
  }
</style>