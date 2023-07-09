<div class="summary">
  <div class="summary__title">Hakkımda</div>

  <div class="summary__content">
    Merhaba ben Yusuf İlker Oğuz, İstanbul/Fikirtepe'de yaşıyorum. En uzun
    süreli deneyemim React kütüphanesinde. Svelte ve Vue Frameworklerinde küçük
    projeler yaptım. Teknoloji ayırt etmeyen birisiyim. Chrome - LightHouse
    kütüphanesini çok sık kullanıyorum. Webpack, Gulp, Grunt, Parcel - bundler 
    kütüphanelerini kullandım. SASS, LESS gibi CSS preprocessorlerini kullandım.
  </div>
</div>

<style lang="scss">
  .summary {
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

    &__content {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      flex-wrap: wrap;
      width: 100%;
      flex: 0 0 100%;
    }
  }
</style>
