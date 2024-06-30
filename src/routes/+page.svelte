<script>
  import { base } from "$app/paths";

  import imgA from "$lib/images/main-page/A.jpg";
  import imgB from "$lib/images/main-page/B.jpg";
  import imgC from "$lib/images/main-page/C.jpg";
  import imgD from "$lib/images/main-page/D.jpg";

  import TopBar from "$lib/components/TopBar.svelte";
  import Contact from "$lib/components/Contact.svelte";
</script>

<TopBar />

<div class="col stretch content-panel">
  <div class="col" style="max-width: 650px">
    <h1>Recambios en Barcelona</h1>
    <p>Recambios Gil Comas es una empresa de Barcelona de largo recorrido especializada en la venta de recambios y accesorios para automóviles. Contamos con un amplio stock de piezas de repuesto para cubrir todas las marcas y modelos. Porque esa es la manera de asegurarnos que vas a recibir tu servicio en poco tiempo. Y para nosotros, es importante que soluciones con celeridad el incómodo problema de tu coche o moto. Por eso, nos gusta ser ágiles.</p>
  </div>
</div>

<div class="triple-panel">
  <div class="col paragraph-panel" style="background: #246c61">
    <h2>Siéntete seguro con tu coche o moto a punto</h2>
    <p>Gracias a nuestra amplia gama de fabricantes de confianza, podrás sentirte seguro al volante. Nuestro abanico de posibilidades en recambios de coches y motos, te brindará la oportunidad de conseguir piezas de calidad.</p>
    <a class="button" href="{base}/contacto">Contacta aquí</a>
  </div>
  <div class="col paragraph-panel" style="background: #80e0d5">
    <h2 style="color:#246c61">Consigue aquí tus recambios de confianza</h2>
    <p style="color:#246c61">Además, nos gusta dar un trato de confianza a todos nuestros clientes. Y eso, lo conseguimos a través de una comunicación clara y un asesoramiento experto, que vaya destinado siempre a mejorar la eficiencia de tu automóvil.</p>
    <a class="button" href="{base}/contacto">Encuéntralos aquí</a>
  </div>
  <div class="col paragraph-panel" style="background: #1e6193">
    <h2>Tu automóvil rendirá más con los recambios de Gil Comas</h2>
    <p>Si ya tienes claro que necesitas no dudes en poner en contacto con nosotros.</p>
    <a class="button" href="tel:+34934909722">Llama ya</a>
  </div>
</div>

<div class="row stretch" style="height: clamp(130px, 35vw, 350px);">
  <img class="image" alt="" src={imgA}/>
  <img class="image" alt="" src={imgB}/>
  <img class="image" alt="" src={imgC}/>
  <img class="image" alt="" src={imgD}/>
</div>

<div class="row stretch" style="background: #bd7b21;padding: 10px">
  <h1 style="max-width:650px">
    ¿Es hora de poner tu coche o moto a punto? Nos
    <a href="{base}/contacto">encantará</a>
    asesorarte sobre recambios
  </h1>
</div>

<Contact/>

<style>
  .image {
    flex-grow: 1;
    height: 100%;
    width: 0px;
    object-fit: cover;
  }
  .content-panel {
    background-image: url("$lib/images/fachada.jpg");
    background-color: rgba(250, 150, 30, .9);
    background-blend-mode: multiply;
    background-size: cover;
    background-position: center;
    padding: min(120px, 10%);
    text-shadow: #000 0px 0 20px, #000 0px 0 20px, #000 0px 0 30px, #000 0px 0 30px;
  }
  
  .triple-panel {
    display: grid;
    grid-template-columns: auto auto auto;
  }

  @media (max-width: 900px) {
    .triple-panel {
      grid-template-columns: auto;
    }
  }

  .paragraph-panel {
    gap: 10px;
    padding: 10% 20% 10% 20%;
  }

  .button {
    background: #fff;
    border-radius: 10000px;
    border: none;
    margin: 18px;
    font-family: Ubuntu;
    font-size: 1.2em;
    padding: 8px 12px 8px 12px;
    color: #0b2521;
    cursor: pointer;
    transition: all 300ms;
  }

  .button:hover {
    color: #fff;
    background: #0b2521;
  }
</style>
