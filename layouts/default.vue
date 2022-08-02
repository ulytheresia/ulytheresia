<template>
  <div class="has-background-primary">
    <div class="container">
      <b-navbar centered class="is-primary">
        <template #brand>
          <b-navbar-item tag="router-link" :to="{ path: '/' }">
            <span class="has-text-weight-bold has-text-danger">/&nbsp;</span>
            <span class="has-text-weight-bold">ULYTHERESIA</span>
          </b-navbar-item>
        </template>
        <template #start>
          <b-navbar-item href="/about" class="px-6"> About </b-navbar-item>
          <b-navbar-item href="/experiences" class="px-6"> Experiences </b-navbar-item>
          <b-navbar-item href="/portfolio" class="px-6"> Portfolio </b-navbar-item>
        </template>

        <template #end>
          <b-navbar-item tag="div">
            <div class="buttons">
              <a class="button px-6 is-secondary" style="border-radius: 10px">
                <strong>Resume</strong>
              </a>
            </div>
          </b-navbar-item>
        </template>
      </b-navbar>
    </div>

    <section class="main-content">
      <div class="container">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      items: [
        {
          title: "Home",
          icon: "home",
          to: { name: "index" },
        },
        {
          title: "Inspire",
          icon: "lightbulb",
          to: { name: "inspire" },
        },
      ],
    };
  },
  methods: {
    scrollTo(a) {
      this.$refs.leadsForm.scrollIntoView();
    }
  }
};
</script>
