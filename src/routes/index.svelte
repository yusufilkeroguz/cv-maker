<script>
  import AboutMe from "../components/AboutMe.svelte";
  import Socials from "../components/Socials.svelte";
  import Skills from "../components/Skills.svelte";
  import Experiences from "../components/Experiences.svelte";
  import References from "../components/References.svelte";
  import Summary from "../components/Summary.svelte";
  import Education from "../components/Education.svelte";
</script>

<div class="container">
  <div class="col">
    <AboutMe />
  </div>
  <div class="col">
    <Socials />
  </div>
  <div class="col">
    <Summary />
  </div>
  <div class="col content">
    <Experiences />
  </div>
  <div class="col right_side">
    <Education />
    <Skills />
    <References />
  </div>
</div>

<style lang="scss">
  .container {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    width: 100%;
    flex-wrap: wrap;
    margin: 0 auto;
    position: relative;
    max-width: 60em;
    background-color: white;
    padding: 2em;
    margin: 0 auto;
    box-sizing: border-box;
  }

  @media screen {
    .container {
      width: 1366px;
    }
  }

  .col {
    flex: 0 0 auto;
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    width: 100%;
    flex-wrap: wrap;

    &.content {
      max-width: 70%;
    }

    &.right_side {
      justify-content: flex-end;
      max-width: 30%;
    }
  }
</style>
