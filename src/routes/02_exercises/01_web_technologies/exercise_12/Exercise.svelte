<script>
	let clicked = false;
</script>


{#if clicked == true}
	<i>You have clicked the button! </i>
{:else}
	<i>You have to click the button!</i>
{/if}

<div>
	<button class="btn btn-primary" on:click={() => (clicked = true)}>
		click here
	</button>
	<!--  -->
	<button class="btn btn-primary" on:click={() => (clicked = false)}>
		unclick
	</button>
</div>
