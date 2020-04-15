<script>
  import FaMapMarkerAlt from 'svelte-icons/fa/FaMapMarkerAlt.svelte'
  import FaBookOpen from 'svelte-icons/fa/FaBookOpen.svelte'
  import FaDonate from 'svelte-icons/fa/FaDonate.svelte'

  import Button from './Button.svelte'
</script>

<div class="row align-items-center justify-content-center secondRowWrapper">
  <div class="col-md-4">
    <div id="rocket" class="background-image"></div>
  </div>
  <div class="col-md-4">
  <div id="thermometer">
    <span class="current">$ 12,000</span>
    <span class="goal">$ 16,000</span>
  </div>
  </div>
  <div class="col-md-4">
    <div class="buttonsWrapper">
      <Button className={"white background-pink"}><div class="icon"><FaBookOpen /></div><span>Learn More<span></Button>
      <Button className={"white background-seafoam"}><div class="icon"><FaDonate /></div><span>Donate<span></Button>
      <Button className={"white background-yellow"}><div class="icon"><FaMapMarkerAlt /></div><span>Google Maps<span></Button>
    </div>
  </div>
</div>

<style>

.secondRowWrapper{
  padding: 2em 0;
}

.secondRowWrapper span{
  /* margin: 1em 0 0 0; */
}

.icon{
  width: 0.75em;
  display: inline-block;
  padding: 0;
  margin: 0 0.5em 0 0;
}

#thermometer{
  margin: 0 auto;
}

.background-image{
	background-size: contain;
	background-repeat: no-repeat;
	background-position: center;
	width: 100%;
}

#rocket{
  height: 20em;
  margin: 0 auto;
  background-image: url(./images/rocket.png)
}

</style>
