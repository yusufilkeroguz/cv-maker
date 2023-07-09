<script>
  const socials = [
    {
      slug: "linkedin",
      label: "/yusuf-ilker-oguz",
      link: "https://www.linkedin.com/in/yusuf-ilker-oguz/",
    },
    {
      slug: "stackoverflow",
      label: "/yusuf-ilker-oğuz",
      link:
        "https://stackoverflow.com/users/2173129/yusuf-%c4%b0lker-o%c4%9fuz",
    },
    {
      slug: "whatsapp",
      label: "+905424553088",
      link: "https://wa.me/+905424553088?text=Hi!",
    },
    {
      slug: "mail",
      label: "yusufilkeroguz@gmail.com",
      link: "mailto:yusufilkeroguz@gmail.com",
    }
  ];
</script>

<div class="socials">
  {#each socials as social}
    <a href={social.link} class={`socials__item ${social.slug}`}>
      <div class="socials__item__img">
        <img
          src={`/icons/${social.slug}.svg`}
          width="24"
          height="auto"
          alt={social.slug}
          align="center"
        />

        {social.label}
      </div>
    </a>
  {/each}
</div>

<style lang="scss">
  .socials {
    flex: 0 0 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: nowrap;
    padding: 0.5rem 0;
    width: 100%;
    border-bottom: 2px solid rgb(46, 46, 46);
    border-right: 0.5rem solid transparent;
    border-left: 0.5rem solid transparent;
    box-sizing: border-box;
    font-family: "Lato", Arial, sans-serif;
    font-size: 1rem;
    color: #000;

    &__item {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      width: auto;
      text-decoration: none;

      img {
        padding-right: 0.25rem;
      }
    }

    @media print {
      font-size: 0.75rem;
    }
  }
</style>
