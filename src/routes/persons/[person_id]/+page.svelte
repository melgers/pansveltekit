<script lang="ts">
	import { page } from '$app/stores';
    import Border from '$lib/pancompany/border.svelte';
    import { findById } from '$lib/stores/persons.js';
       
    const personId = $page.params.person_id;
    const person = findById(Number(personId));
    
</script>

<Border>
<h2>Show details of person {$page.params.person_id}</h2>

{#if person}
    <p>id : {person.id}, name :  {person.name}, age : {person.age}</p>
{/if}
</Border>