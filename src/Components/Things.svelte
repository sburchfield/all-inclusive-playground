<script>

import Pic from './Pic.svelte'

let desc = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."

</script>

<div id="issuesInner">
  <div class="row issuesWrapper justify-content-center">
    <div class="col-lg-4">
      <Pic
        title={"Our Story"}
        description={desc}
        bgColor={'#6CC8C7'}
        image={'./build/images/background.jpg'}
        link={'/Policy#Healthcare'} />
    </div>
    <div class="col-lg-4">
      <Pic
      title={"Why All Inclusive?"}
      description={desc}
      bgColor={'#FDC113'}
      image={'./build/images/background.jpg'}
      link={'/Policy#War_on_Drugs'} />
    </div>
    <div class="col-lg-4">
      <Pic
      title={"Benefits"}
      description={desc}
      bgColor={'#2DAAE1'}
      image={'./build/images/background.jpg'}
      link={'/Policy#Jobs'} />
    </div>
  </div>
  <div class="row issuesWrapper justify-content-center">
    <div class="col-lg-4">
      <Pic
      title={"Contact"}
      description={desc}
      bgColor={'#E82369'}
      image={'./build/images/background.jpg'}
      link={'/Policy#Jobs'} />
    </div>
    <div class="col-lg-4">
      <Pic
      title={"News"}
      description={desc}
      bgColor={'#B933D8'}
      image={'./build/images/background.jpg'}
      link={'/Policy#Jobs'} />
    </div>
  </div>
</div>


<style>
#issuesInner{
  padding: 1em 6em;
}

.issuesWrapper{
  padding: 0 1em;
}


@media (max-width: 1200px){
  #issuesInner{
    padding: 1em;
  }

  .issuesWrapper{
    padding: 0;
  }
}
</style>
