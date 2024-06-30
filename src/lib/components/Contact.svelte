<script>
    import PhoneIcon from "$lib/icons/phone.svelte";
    import MailIcon from "$lib/icons/mail.svelte";
    import LocationIcon from "$lib/icons/location.svelte";
    import ClockIcon from "$lib/icons/clock.svelte";
</script>

<div class="col align-start contacta-panel">
    <h3>CONTACTA CON NOSOTROS</h3>
    
    <div class="dyn-row align-start">
        <div class="col align-start">
            <a class="row" href="tel:+34934909722">
                <PhoneIcon />934909722
            </a>
            <a class="row" href="mailto:rgilcomas@gmail.com">
                <MailIcon />rgilcomas@gmail.com
            </a>
        </div>
    
        <div class="col align-start">
            <div class="row">
                <ClockIcon />
                Lunes - Viernes
                <div style="margin-left: 30px">
                    09:00 - 13:00<br>15:30 - 19:30
                </div>
            </div>
            <a class="row" href="https://www.google.com/maps/place/Recanvis+Gil+Comas/@41.3834767,2.1338216,15z/data=!4m6!3m5!1s0x12a49862e6fd27e9:0xb08b9c525781866d!8m2!3d41.3834767!4d2.1338216!16s%2Fg%2F1tcwb6pg?entry=ttu">
                <LocationIcon />
                Carrer Novell, 62, 08014 Barcelona, BARCELONA
            </a>
        </div>
    </div>
    
    </div>

      
<style>
    .contacta-panel {
        padding: 30px;
    }
    a {
        color: #8ccdff;
    }
    
    .dyn-row {
        gap: 40px;
    }
    @media (max-width:700px)  {
        .dyn-row {
            gap:0px;
            flex-direction: column;
        }
    }
</style>
