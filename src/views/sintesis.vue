<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
   
    p.mb-5 A continuación, encontrará una síntesis de las temáticas abordadas en el componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis-.svg", alt="A continuación, se presenta la síntesis del componente formativo: Estructura del servicio, donde se encuentra el cliente con necesidades y tipos de clientes; el servicio, en conjunto con el ciclo del servicio y políticas del servicio; etiquetas y protocolos con sus respectivos manuales y elementos corporativos. También dentro de la estructura del servicio se encuentran la comunicación, en conjunto con los tipos de comunicación y planes de comunicación; los canales de atención, con los tipos de canales y normatividad; y, por último, se encuentran los medios tecnológicos, como sistemas de información y bases de datos.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
