<script>
    import { base } from "$app/paths";

    import PhoneIcon from "$lib/icons/phone.svelte";
    import MailIcon from "$lib/icons/mail.svelte";
</script>
  

<div class="row stretch links-panel">
    <a class="row" href="mailto:rgilcomas@gmail.com">
        <MailIcon />
        <p class="hide-if-small">rgilcomas@gmail.com</p>
    </a>
    <a class="row" href="tel:+34934909722">
        <PhoneIcon />
        <p class="hide-if-small">934909722</p>
    </a>
    <div class="grow"></div>
    <a class="page-link" href="{base}/">INICIO</a>
    <a class="page-link" href="{base}/productos">PRODUCTOS</a>
    <a class="page-link" href="{base}/contacto">CONTACTO</a>
</div>


<style>
    .links-panel {
      gap: 30px;
      background: #246c61;
      padding: 10px 40px 10px 40px;
    }

    .page-link {
      padding: 3px;
      border-bottom: 1px solid #fff0;
      color: #fff;
      transition: 300ms;
    }
  
    .page-link:hover {
      border-color: #fff;
    }
</style>