<script lang="ts">
    import Border from '$lib/pancompany/border.svelte';


	import Hello from '$lib/pancompany/hello.svelte';

</script>

<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-5">
		<h1 class="h1">Pan company Svelte(kit) Demo</h1>
		<Border>		
			<Hello name="Hans"/>
		</Border>
	</div>
</div>
