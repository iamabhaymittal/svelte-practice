<script>
  import Face from "./Face.svelte";
  let say = 'hi';
</script>
<style>
  div {
    color: red;
  }
  :global(div){
    background-color: blue;
  }
</style>
<div>
  Say: {say}
</div>
<Face size="4"/>
<Face size="14"/>
<Face />