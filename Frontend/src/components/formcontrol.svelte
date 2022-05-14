<div class="imgholder">
	<div class="masking">
		<div class="control">
			<div class="d-grid gap-2 col-6 mx-auto ">
				<button class="btn btn-primary space" type="button"><a href="src\routes\PatientRegistration.svelte">Patient Registration</a></button>
				<button class="btn btn-primary space" type="button"><a href="src\routes\patientDetails.svelte">Patient Details</a></button>
				<button class="btn btn-primary space" type="button">Remove Details</button>
				<button class="btn btn-primary space" type="button">Update Details</button>
			</div>
		</div>
	</div>
</div>

<style>
	.control {
		position: relative;
		top: 30vh;
	}
	.imgholder {
		background-image: url('hospatal.jpg');
		background-size: cover;
		height: 100vh;
		width: 100vw;
	}

	.masking {
		background: rgb(9, 9, 9);
		background: radial-gradient(
			circle,
			rgba(9, 9, 9, 1) 0%,
			rgba(6, 6, 6, 0.45171572046787467) 51%,
			rgba(4, 4, 4, 0.3060574571625525) 100%
		);

		height: 100vh;
		width: 100vw;
	}
	.space {
		margin: 2%;
	}
    a{
        color: white;
		text-decoration: none;
    }
	a:hover{
		color: orange;
	}
</style>
