<script>
	import { onMount } from "svelte";
	let seconds = 2; // Set the number of seconds for the redirection
  
	onMount(() => {
	  const timer = setTimeout(() => {
		window.location.href = "https://egspschools.com";
	  }, seconds * 1000);
  
	  return () => {
		clearTimeout(timer);
	  };
	});
  </script>
  
  
  
  <div id="content">
	<h1>Redirecting to egspschools.com</h1>
	<p>If you are not redirected, <a href="https://egspschools.com">click here</a>.</p>
	<p>Powered by <span> <a href="https://bumblebees.co.in/"> Bumble Bees</a> </span></p>
  </div>
  