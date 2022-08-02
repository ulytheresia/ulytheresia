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
  name: "LayoutForContent"
};
</script>
