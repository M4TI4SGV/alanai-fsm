<script>
	import '../bootstrap.min(2).css';
	import AlanAI from '$lib/AlanAI.svelte';

    let navExpand = false
</script>

<AlanAI />
<nav class="navbar navbar-dark bg-dark navbar-expand-lg bg-light py-2">
	<div class="container">
		<a class="navbar-brand" href="/">
			<strong>Alan</strong> FSM
		</a>

		<button class="navbar-toggler" on:click={()=>{navExpand = !navExpand}}>
			<span class="navbar-toggler-icon" />
		</button>

		<div class="navbar-collapse" id="navshow" style="display: {(navExpand) ? 'block' : 'none'}">
			<ul class="navbar-nav">
				<li class="nav-tiem">
					<a href="/" class="nav-link">Home</a>
				</li>
				<li class="nav-tiem">
					<a href="/login" class="nav-link">Login</a>
				</li>
				<li class="nav-tiem">
					<a href="/dashboard" class="nav-link">Dashboard</a>
				</li>
			</ul>
		</div>
	</div>
</nav>
<AlanAI/>

<slot />
