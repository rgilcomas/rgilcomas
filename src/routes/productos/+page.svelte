<script>
    import { base } from "$app/paths";
  
    import imgA from "$lib/images/productos/A.jpg";
    import imgB from "$lib/images/productos/B.jpg";
    import imgC from "$lib/images/productos/C.jpg";
  
    import Contact from "$lib/components/Contact.svelte";
    import TopBar from "$lib/components/TopBar.svelte";
</script>

<TopBar />

<div class="col stretch content-panel">
    <h1>Recambios de coches en Barcelona</h1>
</div>

<div class="text-panel">
Es totalmente normal que al pasar los años, <b>algunas piezas de tu vehículo comiencen a fallar</b> y haya que reemplazarlas por otras nuevas. Y es que esta es la manera en la que podemos seguir utilizando nuestro vehículo o moto, y alargar así su vida. De otra forma, habría que comprar uno nuevo.
<br><br>
Pero ¿Sabes lo que hay que tener en cuenta a la hora de elegir tus recambios? Mi recomendación es que, antes de nada, un mecánico de confianza o alguno de nuestros expertos te ayude a identificar la pieza que está fallando.
</div>


<div class="col stretch" style="background:#1e6193">
    <div class="dyn-row img-container">
    <img src={imgA} alt=""/>
    <div class="col align-start">
        <h2>No dejes que te engañen por ahí</h2>
        <p>Ten en cuenta que por el mercado hay muchos recambios de dudosa procedencia o repuestos piratas. Y créeme que esos, no te interesan. Te aconsejo que compres tus piezas en lugares de confianza, y nosotros queremos ofrecerte esa seguridad con total franqueza.</p>
    </div>
    </div>
</div>
<div class="col stretch" style="background:#246c61">
    <div class="dyn-row img-container">
    <div class="col align-start">
        <h2>Siente la seguridad de comprar un recambio de calidad</h2>
        <p>En Gil Comas vas a poder encontrar recambios para todas las marcas de coches y motos. Queremos mostrarte nuestra extensa gama de piezas de repuesto, neumáticos, bombillas, aceites de motor, productos de limpieza, herramientas y accesorios para tu vehículo. Para que puedas elegir con nuestra ayuda lo que más te convenga en cada momento.</p>
    </div>
    <img src={imgB} alt=""/>
    </div>
</div>
<div class="col stretch" style="background:#80e0d5;color:#246c61">
    <div class="dyn-row img-container">
    <img src={imgC} alt=""/>
    <div class="col align-start">
        <h2>Con nosotros tendrás acceso a las mejores opciones del mercado de recambios:</h2>
        <p style="color:#246c61">- Lubricantes, aditivos y químicos.<br>
            - Pintura.<br>
            - Neumáticos.<br>
            - Accesorios.<br>
            - Herramientas para automóvil y motos.<br><br>
            Todas las dudas que te surjan, las puedes solucionar con cualquiera de nuestros expertos en mecánica. Estamos a tu entera disposición.
        </p>
    </div>
    </div>
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

    img {
      height: 200px;
      width: min(400px, 30%);
      object-fit: cover;
      flex-shrink: 0;
      border-radius: 40px;
      box-shadow: #fff 0 0 10px, #fff 0 0 5px;
    }

    @media (max-width:700px)  {
        img {
            width: min(400px, 90%);
        }
        .dyn-row {
            flex-direction: column;
        }
    }

    .img-container {
        max-width: 1300px;
        gap: 60px;
        padding: 60px;
    }

    .content-panel {
      background-image: url("$lib/images/fachada.jpg");
      background-size: cover;
      background-position: center;
      padding: 100px;
      text-shadow: #000 0px 0 20px, #000 0px 0 20px, #000 0px 0 30px, #000 0px 0 30px;
    }
    
    .text-panel {
        max-width: 1000px;
        padding: 60px;
    }
</style>
  
