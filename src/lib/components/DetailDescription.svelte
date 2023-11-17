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
                <img src={image} alt="stekje image" loading="lazy" max-width="00" />            
		</div>
	</div>

	<div class="beschrijving">
		<h2>Beschrijving</h2>
		<p>Een van de makkelijkste planten om te verzorgen en stekken, groeit als kool (ook in de koudere maanden) en heeft prachtige paars-groene blaadjes met een glinstering.</p>
	</div>
</div>

<style>

.container {
    display: flex;
    flex-direction: column;
    border-radius: 10px;
    overflow: hidden;
    padding: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    margin-top: 4rem;
}

.image-container img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.titel {
    font-size: large;
    padding: 10px;
    text-align: center;
    width: 100%;
}

.beschrijving {
    padding: 20px;
}

.beschrijving h2 {
    color: var(--color-primair);
    margin-bottom: 10px;
    text-transform: uppercase;
}

/* Media Query voor schermen groter dan 768px */
@media screen and (min-width: 768px) {
    .container {
        flex-direction: row;
    }

    .image-container {
        margin-right: 20px;
    }
}

/* Media Query voor schermen groter dan 1024px */
@media screen and (min-width: 1024px) {
    .content-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}
    .image-container {
        width: 300px;
    }
    .beschrijving {
        max-width: 35rem;
    }
}
</style>
