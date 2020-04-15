<script>

</script>

<div class="container">
	<header>
		<div class="filter">
			<div class="row headerWrapper justify-content-center align-items-center">
				<div class="col-3">
					<div id="rotary" class="headerImages"></div>
				</div>
				<div class="col-6">
					<div class="text-center">
							<h1>DaVinici's</h1>
							<h2>All Inclusive Playground</h2>
							<h3><span>All Inclusive</span><span>All Ages</span><span>All Welcome</span></h3>
							<h4>4321 Playground Ave</h4>
							<h4>Oak Ridge, Tn</h4>
					</div>
				</div>
				<div class="col-3">
					<div id="lap" class="headerImages"></div>
				</div>
			</div>
		</div>
	</header>
</div>

<style>
header{
  background-image: url(./images/background.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size:cover;
  height:26em;
  color: #fff;
}

header h1{
	font-size: 3.5em;
  font-weight: bold;
}

header h2{
  font-weight: 300;
	font-size: 2.5em;
}

header h3{
	font-size: 1.5em;
	font-weight: 200;
}

header h3 span{
	padding: 0 0.5em 0 0.5em;
}

header h4{
	font-size: 1.25em;
	font-weight: 200;
}

.filter{
  position: relative;
  width: 100%;
  height: 100%;
  background: rgba(39,62,116,0.7);
  z-index: 50;
}

.headerWrapper{
  padding-top: 3em;
}

.header-donate-btn{
  background-color: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 1);
  display: block;
  margin: 4em auto 0 auto;
  padding: 1em 2.5em;
}

.header-donate-text{
  text-align: center;
  font-weight: normal;
  margin: 1em 0 0 0;
}

.headerImages{
	background-size: contain;
	background-repeat: no-repeat;
	background-position: center;
	width: 100%;
}

#rotary{
	height: 18em;
	background-image: url(./images/Rotary.png);
}

#lap{
	height: 19.5em;
	background-image: url(./images/letsAllPlay.png);
}

@media only screen and (max-width: 838px) {
	header h1{
		font-size: 2em;
	}

	header h2{
		font-size: 0.9em;
	}

	header h3{
		font-size: 0.5em;
	}

	header h3 span{
		padding: 0 0.25em 0 0.25em;
	}

	header h4{
		font-size: 0.3em;
	}

}

</style>
