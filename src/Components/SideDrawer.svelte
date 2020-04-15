<script>
  export let show;
</script>


<nav class={show}>
  <ul>
    <li><a href="#" on:click>Home</a></li>
    <li><a href="#" on:click>Sponsors</a></li>
    <li><a href="#" on:click>News</a></li>
    <li><a href="#" on:click>Contact</a></li>
    <li><a href="#" on:click>Gallery</a></li>
    <li><a href="#" on:click>Donate</a></li>
  </ul>
</nav>

<style>
.sideDrawer{
  height: 100%;
  background: #fff;
  box-shadow: 1px 0px 7px rgba(0,0,0,0.5);
  position: fixed;
  top: 0;
  left: 0;
  width: 70%;
  max-width: 400px;
  z-index: 1000;
  transform: translateX(-100%);
  transition: transform 0.3s ease-out;
  padding-left: 2em;
}

.sideDrawer.open{
  transform: translateX(0);
}

.sideDrawer ul{
  height: 100%;
  list-style: none;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.sideDrawer li{
  margin: 0.5em 0;
}

.sideDrawer a{
  color: rgba(0, 0, 0, 1);
  text-decoration: none;
  font-size: 1.2em;
}

.sideDrawer a:hover, .sideDrawer a:active {
  color: rgba(0,0,0,0.5);
}

@media (min-width: 769px){
  .sideDrawer{
    display: none;
  }
}
</style>
