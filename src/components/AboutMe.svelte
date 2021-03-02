<div class="about-me">
  <div class="about-me__left">
    <h1 class="name">Yusuf İlker Oğuz</h1>
    <h2 class="job-title">Frontend Developer</h2>
  </div>
  <div class="about-me__right">
    <img src="/sexy-me.jpg" alt="Yusuf İlker Oğuz" width="150" height="auto" />
  </div>
</div>

<style lang="scss">
  .about-me {
    flex: 0 0 100%;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    flex-wrap: nowrap;
    width: 100%;
    padding-bottom: 0.5rem;
    border-bottom: 2px solid rgb(46, 46, 46);
    border-right: 0.5rem solid transparent;
    border-left: 0.5rem solid transparent;
    box-sizing: border-box;
    font-family: "Lato", Arial, sans-serif;
    font-size: 1rem;
    color: #000;

    .name {
      font-size: 4rem;
      font-weight: bold;
      margin: 0 0 0.75rem 0;
    }

    .job-title {
      font-size: 3rem;
      margin: 0;
    }
  }
</style>
