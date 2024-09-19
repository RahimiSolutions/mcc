<script>
	import Logo from './Logo.svelte';
import MediaQuery from './MediaQuery.svelte';
</script>

<MediaQuery query="(min-width: 936px)" let:matches>
	{#if matches}
		<nav>
			<div class="logo">
                <Logo />
            </div>
			<div class="navbar-menu">
				<ul>
					<li><p>Bønnetabell</p></li>
					<li><p>Om MCC</p></li>
					<li><p>Kontakt</p></li>
				</ul>
			</div>
			<div class="navbar-cta">
				<p>Støtt MCC</p>
			</div>
		</nav>
	{/if}
</MediaQuery>

<style>
	
	nav{
		display: flex;
		justify-content: space-between;
		max-height: 75px;
		width: 100%;
		padding: 0 10% 0 10%;
		border: 1px solid red;
	}

	.navbar-menu{
		display: flex;
		align-items: center;
	}
	.navbar-menu ul{
		display: flex;
		list-style-type: none;
	}

	ul li{
		margin: 10px;
	}
	
</style>