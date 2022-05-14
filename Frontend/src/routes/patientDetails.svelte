<script>
    import { onMount } from 'svelte';
    let Details;

    onMount(async () => {
        const response = await fetch("http://localhost:8080/");
        const data = await response.json();
        Details = data.name;
        
    })
</script>

<main>
    <h1>WORKING</h1>
    {Details}
</main>
      