<script>
    import Navbar from "../components/Navbar.svelte";
</script>

<Navbar/>
<slot />

<style>
    :global(*) {
		/* --primary: #080a16;
		--secondary: #f4fffd;
		--contrast: #12141f;
		--detail: #f8de7e; */
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		
	}
	:global(p){
		font-family: 'Poppins';		
		src: local('$lib/fontfaces/Poppins-Regular.ttf');
	}
</style>