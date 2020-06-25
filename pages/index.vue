<template>
  <section class="section">
    <h1>Hello world !</h1>
    <div class="columns is-mobile">

      <card class="column"
        title="Free"
        icon="github-circle"
      >
        Open source on <a href="https://pcweb-conseils.com"> Pcweb</a>
      </card>

      <card class="column"
        title="Responsive"
        icon="cellphone-link"
      >
        <b class="has-text-grey">Every</b> component is responsive
      </card>

      <card class="column"
        title="Modern"
        icon="alert-decagram"
      >
        Built with <a href="https://vuejs.org/">Vue.js</a> and <a href="http://bulma.io/">Bulma</a>
      </card>

    </div>
  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>
