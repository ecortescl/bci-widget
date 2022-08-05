<template>
<div class="m-4">
    <h1 class="text-center">Ejemplo de Uso widget BCI</h1>
    <h3 class="text-center"> Pre aprobacion Bancaria</h3>
    <hr>

    <div class="row justify-content-center">
        <div class="col-lg-4 text-center">
            <b-button v-b-modal.modal-1>OBTÉN TU PREAPROBACIÓN EN LÍNEA</b-button>

            <b-modal id="modal-1" title="BCI"  centered  hide-footer>
                <bci-widget api-key="48LAkDa1fiAC7w0DN6AmcmHN3mAfC4Cb" proyecto="Iniciativa Dharma" vendedor="Inmobiliaria" rut="111111111" tipo-propiedad="casa" antiguedad-propiedad="nueva" precio-propiedad="3000" user-id="portal-id" email="ejemplo@micorreo.com" fecha-intencion-compra="02-02-2021" duracion-credito="20" telefono="+56999999999">
                </bci-widget>
            </b-modal>
        </div>
    </div>

</div>
</template>

<script>
export default {
    name: 'IndexPage',

    head: {
        script: [{
            src: 'https://personas.bci.cl/nuevaWeb/fe-ecochip-widget-sandbox/bci-widget.js',
            defer: true,
            crossorigin: "anonymous"
        }],

    }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Overpass:wght@600&display=swap');
.btn-secondary{
  background-color: #37474F !important;
  font-family: 'Overpass', sans-serif;
  font-size:16px;

}
body{
  font-family: 'Overpass', sans-serif;
}
  
</style>
