<script>
  const experiences = [
    {
      companyName: `PropertyFinder`,
      title: `Frontend Developer`,
      date: `Apr 2021 - Current`,
      desc: `PropertyFinder is biggest property finder platform for Saudi Arabia. In PropertyFinder i am working on in office projects(Admin Page, SAAS Panel). In office projects are written with React & SPA (Single Page App.). Also using TS (TypeScript), Webpack, BEM Css.`,
    },
    {
      companyName: `Modanisa`,
      title: `Frontend Developer`,
      date: `Nov 2019 - Apr 2021`,
      desc: `Modanisa has big structure and Modanisa converted monolith structure to micro structure. I wrote Layout Service (All products connected to layout ). I am currently using React, Gulp, Webpack, SASS, MaintableCSS.`,
    },
    {
      companyName: `Enuygun`,
      title: `Frontend Developer`,
      date: `Apr 2018 - Nov 2019`,
      desc: `Enuygun called me when i resigned at Kolay Randevu. I started as Frontend Developer at Enuygun again. I was Hotel and Blog teams at Enuygun. I wrote React, Webpack, Autoprefixer, SASS etc.`,
    },
    {
      companyName: `Kolay Randevu`,
      title: `Frontend Developer`,
      date: `Jun 2017 - Apr 2018`,
      desc: `Kolay Randevu is a startup about appointment hairdresser. I was alone as Frontend Developer at Kolay Randevu. I created structure with Webpack, Grunt, jQuery, Babel, SASS etc.`,
    },
    {
      companyName: `Enuygun`,
      title: `Frontend Developer`,
      date: `Jun 2012 - Jan 2017`,
      desc: `I was intern at 2012, After intern i started at Enuygun as Full Stack Developer. In 2013, I wanted to change my role as Frontend Developer and Enuygun changed my role to Frontend Developer. I wrote jquery, gulp, SASS, grunt from 2012 to 2015, In 2015 i learned React. Since 2015 i write React.`,
    },
  ];
</script>

<div class="experiences">
  <div class="experiences__title">Experiences</div>

  {#each experiences as experience}
    <div class="experience">
      <div class="experience__company-name">
        {experience.companyName}
      </div>
      <div class="experience__title">
        {experience.title}
      </div>
      <div class="experience__date">
        {experience.date}
      </div>
      <div class="experience__desc">
        {experience.desc}
      </div>
    </div>
  {/each}
</div>

<style lang="scss">
  .experiences {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    width: 100%;
    flex-wrap: wrap;
    padding-top: 1rem;
    box-sizing: border-box;
    font-family: "Lato", Arial, sans-serif;
    font-size: 1rem;
    color: #000;

    &__title {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      padding: 0.25rem;
      font-size: 2rem;
      font-weight: bold;
      border-bottom: 2px solid #000;
      border-right: 0.5rem solid transparent;
      border-left: 0.5rem solid transparent;
      margin-bottom: 0.25rem;

      img {
        padding-right: 0.25rem;
      }
    }
  }

  .experience {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    width: 100%;
    flex-wrap: wrap;
    padding-top: 1.55rem;
    font-size: 1.25rem;

    &__company-name {
      flex: 0 0 100%;
      font-size: 1.5rem;
      font-weight: 500;
    }

    &__title {
      flex: 0 0 100%;
      font-weight: 500;
    }

    &__date {
      flex: 0 0 100%;
      font-size: 1rem;
    }

    &__desc {
      flex: 0 0 100%;
      font-size: 1rem;
    }
  }
</style>
