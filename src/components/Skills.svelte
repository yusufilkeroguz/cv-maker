<script>
  const skills = [
    "React",
    "Vue",
    "Svelte",
    "Sass",
    "jQuery",
    "Bootstrap",
    "Material UI",
    "Redux",
    "Docker",
    "Node JS",
    "MobX",
  ];

  const slugify = (name) => name.replace().toLowerCase().replace(/\s+/g, "-");
</script>

<div class="skills">
  <div class="skills__title">Skills</div>
  {#each skills as skill}
    <div class="skill {skill}">
      <img
        src="/icons/{slugify(skill)}.svg"
        alt={slugify(skill)}
        width={24}
        height="auto"
      />

      {skill}
    </div>
  {/each}
</div>

<style lang="scss">
  .skills {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    width: 100%;
    flex-wrap: wrap;
    padding-top: 1rem;
    box-sizing: border-box;
    font-family: "Lato", Arial, sans-serif;
    font-size: 1.25rem;
    color: #000;

    &__title {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      padding: 0.25rem;
      font-size: 2rem;
      font-weight: bold;
      border-bottom: 2px solid #000;
      border-right: 0.5rem solid transparent;
      border-left: 0.5rem solid transparent;
      margin-bottom: 0.25rem;
    }

    .skill {
      flex: 0 0 100%;
      display: flex;
      justify-content: flex-end;
      align-items: center;
      flex-wrap: nowrap;
      padding: 0.25rem;

      img {
        padding-right: 0.25rem;
      }
    }
  }
</style>
