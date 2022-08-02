<template>
  <div class="wrapper">
    <section class="section hp-section">
      <div class="columns is-mobile is-centered">
        <div class="column has-text-centered">
          <div class="title-hp py-3">
            <h2 class="is-size-5">Hi, my name is</h2>
          </div>
          <div class="mt-3">
            <h1>Uly Theresia.</h1>
            <div class="vector-hp">
              <img src="../assets/Vector.png" alt="vector" />
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section pt-1">
      <div class="columns is-mobile is-centered">
        <div class="column is-half has-text-centered">
          More than 3 years in programming, speciﬁcally front-end. Motivated to
          grow and develop my skills and my knowledge, especially
          product-related thing
        </div>
      </div>
      <div class="columns is-mobile is-centered">
        <div class="column has-text-centered">
          <b-button
            class="
              has-background-black has-text-white
              px-6
              has-text-weight-bold
            "
            >Contact Me</b-button
          >
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  components: {},
};
</script>
<style lang="scss" scoped>
.wrapper {
  min-height: 100vh;
  .hp-section {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-top: 15%;
  }
  .title-hp {
    background: rgba(255, 255, 255, 0.6);
    border: 1px solid #e4e4e7;
    backdrop-filter: blur(14px);
    border-radius: 60px;
    padding-left: 8rem;
    padding-right: 8rem;
  }
  h1 {
    color: #18181b;
    font-weight: 800;
    font-size: 52px;
    line-height: 62px;
  }
}
@media screen and (max-width: 520px) {
  .wrapper {
    .title-hp {
      padding-left: 3rem;
      padding-right: 3rem;
    }
  }
}
</style>
