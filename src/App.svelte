<script>
	import Header from './Components/Header.svelte'
	import Nav from './Components/Nav.svelte'
	import SideDrawer from './Components/SideDrawer.svelte'
	import Backdrop from './Components/Backdrop.svelte'
	import SecondRow from './Components/SecondRow.svelte'
	import Statement from './Components/Statement.svelte'
  import Things from './Components/Things.svelte'
	import RotaryService from './Components/RotaryService.svelte'
	import Statements from './Components/Statements.svelte'
	import Footer from './Components/Footer.svelte'

	let show = false;
	let drawerClasses = 'sideDrawer'

	function drawerToggleHandler(){
		show = !show
		if(show){
			drawerClasses = 'sideDrawer open'
		}else{
			drawerClasses = 'sideDrawer'
		}
	}

</script>

<Header />
<Nav on:click={drawerToggleHandler} />
<SideDrawer show={drawerClasses} on:click={drawerToggleHandler}/>
{#if show}
<Backdrop on:click={drawerToggleHandler} />
{/if}
<SecondRow />
<Statement />
<Things />
<RotaryService />
<Statements />
<Footer />
