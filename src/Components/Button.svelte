<script>
  export let className = false;
</script>


<button class={className}>
  <slot></slot>
</button>

<style>

  button{
    display: block;
    font-size: 1.2em;
    width: 80%;
    margin: 0.5em auto;
    border-radius: 6px;
    padding: 0.25em 0 0.25em 25%;
    box-shadow: 0px 2px 3px rgba(0,0,0,0.02);
    text-align: left;
  }

  @media only screen and (max-width: 1080px) {
    button{
      padding: 0.25em 0 0.25em 20%;
    }
  }

  @media only screen and (max-width: 1080px) {
    button{
      padding: 0.25em 0 0.25em 15%;
    }
  }

    @media only screen and (max-width: 1080px) {
      button{
        padding: 0.25em 0 0.25em 25%;
      }
    }


</style>
