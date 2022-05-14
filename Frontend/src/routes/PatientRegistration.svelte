<script>
	import Footer from '../components/footer.svelte';
	import Navbar from '../components/navbar.svelte';
	import PatientEntry from '../components/PatientEntry.svelte';
    export let firstName = "";
    export let lastName = "";
    export let Age = "";
    export let Gender = "";
    function submitSearch(){
        goto("/search"+firstName)
    }
</script>

<h1>WORKING!</h1>

<Navbar />

<div class="design">
	<form onsubmit={submitSearch  } action="">
        <div class="fix">
		<label class="space" for="Patient Name">Enter your First Name: </label>
		<input bind:value={firstName} class="space" type="text" name="" id="" />
        <br>
		<label class="space" for="Patient Name">Enter your Last Name: </label>
		<input bind:value={lastName} class="space"type="text" name="" id="" />
        <br>
		<label class="space " for="Patient Name">Enter your Age   : </label>
		<input bind:value={Age} class="space align" type="text" name="" id="" />
        <br>
		<label class="space" for="Patient Name">Enter your Gender: </label>
		<input bind:value={Gender} class="space" type="text" name="" id="" />
        <button>Submit</button>
    </div>
	</form>
</div>

<Footer />

<style>
	.fix {
		display: block;
        border: 2.5px solid black;
        height: 75vh;
        width: 50vw;
        
	}
    .space{
        margin: 5%;

    }
    .design{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .align{
        margin-left: 5%;
    }
</style>
