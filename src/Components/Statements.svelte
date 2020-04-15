<script>
  import ColorCard from './ColorCard.svelte'
</script>

<div class="row statementsWrapper justify-content-center">
  <div class="col-lg-4">
    <ColorCard className="background-pink">
      <h4 class="text-center" slot="header">Promoting Peace</h4>
      <p>By supporting a playground for all, without exclusion. Rotary promotes understanding of others encourages peaceful acceptance.</p>
    </ColorCard>
  </div>
  <div class="col-lg-4">
    <ColorCard className="background-blue">
      <h4 class="text-center" slot="header">Supporting Education</h4>
      <p>The Oak Ridge daVinci All-Inclusive Playground will foster education through play. How appropraite for Oak Rdige to have a playground whose theme is "The Art and Science of Play."</p>
    </ColorCard>
  </div>
  <div class="col-lg-4">
    <ColorCard className="background-seafoam">
      <h4 class="text-center" slot="header">Growing Local Economies</h4>
      <p>Rotary recognizes that community playgrounds draw families from surrounding communities and promote city commerce.</p>
    </ColorCard>
  </div>
</div>

<style>
  .statementsWrapper{
    padding: 2em 0;
  }

  p{
    width: 80%;
    margin: 0 auto;
    text-align: left;
    text-indent: 1.25em;
  }
</style>
