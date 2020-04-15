<script>
  export let image;
  export let title;
  export let description;
  export let bgColor;
  export let link = false;

  let fontColorValue = '#fff';
  let linkColorValue = 'white';
  let infoBgStyle = `top: 75%; background-color: ${bgColor};`
  let headerStyle = 'padding: 0.75em 0 1em 0';
  let bgImage = `background-image: url(${image});`

  function setInfoBgStyleUp(){
    infoBgStyle = `top: 0; background-color: ${bgColor};`
  }

  function setInfoBgStyleDown(){
    infoBgStyle = `top: 75%; background-color: ${bgColor};`
  }
</script>

  <div on:mouseover={setInfoBgStyleUp} on:mouseout={setInfoBgStyleDown} class="galleryImage" style={bgImage}>
    <div class="infoBackground" style={infoBgStyle}>
      <h4 class="bold" style={headerStyle}>{title}</h4>
      <p class="paragraph">{description}</p>
      <a href={link}>More...</a>
    </div>
  </div>


<style>
.galleryImage{
  width: 100%;
  height: 16em;
  border-radius: 12px;
  padding: 0;
  margin: 1em 0;
  box-shadow: 5px 3px 6px rgba(0,0,0,0.1);
  background-color: #000;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  -webkit-transition: background-image 750ms;
  transition: background-image 750ms;
  overflow: hidden;
  text-align: center;
}

.infoBackground{
  color: #fff;
  position: relative;
  width: 100%;
  margin-bottom: 0;
  margin-right: auto;
  margin-left: auto;
  text-align: center;
  transition: top 750ms ease-out;
  height: 100%;
}

.infoBackground h4{
  margin: 0;
  transition: padding 750ms ease-out;
}

.infoBackground p{
  width: 80%;
  margin: 0 auto 0.75em auto;
  font-size: 0.975em;
}

.infoBackground a {
  color: #fff;
  font-weight: bold;
  font-size: 1em;
}

.infoBackground a:hover {
  /* color: blue; */
}

@media (max-width: 1024px){
  .infoBackground p{
    font-size: 1em;
  }
}

@media (max-width: 600px){
  .infoBackground p{
    font-size: 0.8em;
  }
}
</style>
