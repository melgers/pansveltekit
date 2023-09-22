<script lang="ts">
    import Border from "$lib/pancompany/border.svelte";
import Hello from "$lib/pancompany/hello.svelte";
    import { persons } from "$lib/stores/persons";
</script>

<Border>
{#each $persons as person}
    <div>        
        <Hello name={person.name}/><a href={"./persons/"+person.id}>Info</a>
    </div>
{/each}
</Border>