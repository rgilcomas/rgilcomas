<script>
    import { base } from "$app/paths";
  
    import TopBar from "$lib/components/TopBar.svelte";
    import Map from "$lib/components/Map.svelte";
    import Contact from "$lib/components/Contact.svelte";
</script>

<TopBar />

<Map />

<div class="text-panel row grow stretch">
    <div class="text-content">
    <h1 style="color:#246c61">Contacta con Recambios Gil Comas en Barcelona</h1>
    En este momento puede que estés preguntando por qué Gil Comas puede ser <b>tu mejor opción para comprar tus recambios.</b> Y en este punto, te diré que gracias a mis clientes este negocio ve la luz día a día. Y solo por eso, a ellos me debo. Por lo tanto, pienso ganarme tu confianza para que juntos sigamos avanzando, tú con tu coche y yo con mi negocio.
    <h1 style="color:#1e6193">¡Gracias por estar ahí!</h1>
    </div>
</div>


<Contact />
  
<style>    
    .text-content {
        max-width: 1200px;
        padding: 60px;
    }
    .text-panel {
        color: #000;
        background: #eee;
    }

    .text-content h1 {
        font-size: 3em;
    }
</style>
  