<script>

import image from "$lib/assets/scindapsus.jpg";

</script>

<div class="container">
	<div class="content-container">
		<div class="titel">
			<h1>Tradescantia zebrina ‘Vaderplant’
            </h1>
		</div>
		<div class="image-container">
            <img src= {image}  alt="stekje image" loading="lazy" />
		</div>
	</div>

	<div class="beschrijving">
		<h2>Beschrijving</h2>
		<p>Een van de makkelijkste planten om te verzorgen en stekken, groeit als kool (ook in de koudere maanden) en heeft prachtige paars-groene blaadjes met een glinstering.</p>
	</div>
</div>

<style>
	.beschrijving {
		padding: 20px;
	}
	.beschrijving h2 {
		color: var(--color-primair);
		margin-bottom: 10px;
		text-transform: uppercase;
	}
	.content-container,
	.titel {
		display: flex;
	}
    
	/* HIER KOMT DE MEDIA QUERY'Z */

	@media screen and (min-width: 525px) {
		.content-container,
		.titel {
			display: block;
		}

		.image-container {
			display: block;
		}

		/* met deze code maak ik de image Naast de beschrijving text */
		.container {
			display: flex;
			border-radius: 10px;
			overflow: hidden; /* Zorgt ervoor dat de afbeelding binnen de container blijft */
			padding: 10px;
			box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
			margin-top: 4rem;
		}

		.image-container img {
			width: 300px;
			height: auto;
			border-radius: 10px;
		}

		.content-container {
			display: flex;
			flex-direction: column;
			align-items: center;
		}

		.titel {
			font-size: large;
			padding: 10px;
			text-align: center;
			width: 100%;
		}

		.beschrijving {
			display: flex;
			flex-direction: column;
			margin: 28px; /* dit kan op een andere MANIERRR */
			max-width: 35rem;
		}
	}
	@media screen and (min-width: 525px) {
		.container {
			margin-top: none;
		}
	}
</style>
