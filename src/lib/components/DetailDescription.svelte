<script>
    import image from "$lib/assets/scindapsus.jpg";
//     import { onMount } from 'svelte';
//     import { fade } from 'svelte/transition';
//     let isVisible = false;
   
//     onMount(() => {
//      setTimeout(() => {
//        isVisible = true;
//     }, 140);
// });
</script>
  
<article class="container">
    <div class="content-container">
      <div class="title">
        <h1>Epipremnum pinnatum</h1>
      </div>
      <div class="image-container">
        <img src={image} alt="Epipremnum pinnatum stekje" loading="lazy" style="max-width: 300px;" />
      </div>
    </div>
  
    <div class="description" >
        <h2 class="sub-heading">Beschrijving</h2>
      <p> 
        De Epipremnum pinnatum, ook wel Scindapsus Epipremnum genoemd, is een populaire hang- en klimplant. Zorg er voor dat de grond altijd lichtvochtig is, zonder dat er water onder in de pot blijft staan. 
        Zet de plant op een plek zonder direct zonlicht. De Epipremnum komt van nature voor in het bosgebied in Zuidoost-Azië,
        hier kunnen de bladeren wel 90cm groot worden. In deze bosgebieden groeit de Epipremnum, in de schaduw, als een klimplant langs de bomen omhoog. 
        De Scindapsus komt voor in kleuren variërend van groen, geel en wit. De Scindapsus staat in de top-10 van de meest luchtzuiverende planten. 
        De Scindapsus heeft huidmondjes in de bladeren, die schadelijke gassen opnemen en vervoeren door de stengel naar de wortels. 
        Miljarden micro-organismen breken vervolgens deze schadelijke gassen af, die de plant vervolgens gebruikt als voeding.
        Bij dit proces komen geen afvalstoffen of schadelijke gassen vrij.      
      </p>
    </div>
</article> 
  
  <style> 
    .container {
      display: flex;
      flex-direction: column;
      border-radius: 10px;
      overflow: hidden;
      padding: 20px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      margin: 2rem;
      background-color: #fff;
      transition: box-shadow 0.3s ease-in-out;
    }
  
    .image-container {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .image-container img {
       border-radius: 10px;
       max-width: 100%;
       height: auto;
    }
  
    .title {
        font-size: 1.5rem;
      text-align: center;
      margin-bottom: 10px;
    }

    .description {
      padding: 20px;
      text-align: center;
    }

    .description p{
      line-height: 1.5;
    }
  
    .sub-heading {
      color: var(--sub-heading-color);
      margin-bottom: 10px;
      text-transform: uppercase;
    }

 /* .description-text {
      transition: opacity 0.2s ease-in-out;
      opacity: 0;  
    } */

    /* Hover-effect voor container */
    .container:hover {
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
    }
  
    /* Media Query voor schermen groter dan 768px */
    @media screen and (min-width: 768px) {
      .container {
        flex-direction: row;
      }
  
      .image-container {
        margin-right: 20px;
      }
  
      .description {
        text-align: left;
      }
    }
  
    /* Media Query voor schermen groter dan 1024px */
    @media screen and (min-width: 1024px) {
      .content-container {
        display: flex;
        flex-direction: column-reverse;
        align-items: center;
        text-align: center;
      }
  
      .image-container {
        width: 300px;
      }
  
      .description {
        max-width: 45rem;
        margin-left: 0px;
      }
    }  
  </style>
  
  
