<script>
  import DrawerToggleButton from './DrawerToggleButton.svelte';
</script>

<section class="toolbar background-blue">
  <nav class="toolbar_nav" id="toolbar_nav">
  <DrawerToggleButton on:click />
  <div class="row justify-content-center toolbar_nav_items white">
      <div><a href="#">Home</a></div>
      <div><a href="#">Sponsors</a></div>
      <div><a href="#">News</a></div>
      <div><a href="#">Contact</a></div>
      <div><a href="#">Gallery</a></div>
      <div><a href="#">Donate</a></div>
  </div>
  </nav>
</section>

<style>
.toolbar{
  width: 100%;
  z-index: 300;
  padding: 1em 0;
}

.toolbar_nav_items div{
  text-align: center;
  width: 10%;
}

.toolbar_nav_items a{
  font-size: 1.3em;
  color: white;
  text-decoration: none;
}

.toolbar_nav_items a:hover{
  text-decoration: underline;
}

@media (max-width: 768px){
  .toolbar{
    padding: 0.25em 0 0 0;
  }

  .toolbar_nav_items div{
    display: none;
  }

}
</style>
