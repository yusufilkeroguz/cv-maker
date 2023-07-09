<script>
  const experiences = [
    {
      companyName: `RUUF`,
      title: `Frontend Developer`,
      date: `02.2022 - 04.2023`,
      desc: `Burada iki proje bulunuyordu. Admin ve Landing. Tüm projelerin önyüzünde NextJS, Typescript, Docker teknolojilerini kullandım. Admin Projesinde Tailwind, Landing projesinde Material-UI kullandım.`,
    },
    {
      companyName: `PropertyFinder`,
      title: `Frontend Developer`,
      date: `07.2021 - 02.2022`,
      desc: `Admin takımında idim. Tüm admin(ev silme, ev ekleme, mütaahit ekleme gibi) adımlarının önyüzünü yapıyordum. Admin projemiz CRA, Webpack, SASS, Typescript teknolojilerini kullandım. CSS Methodolojisi olarak BEM kullandım.`,
    },
    {
      companyName: `Modanisa`,
      title: `Frontend Developer`,
      date: `11.2019 - 05.2021`,
      desc: `Ödeme ve sonrası takımında idim. Ödemeler, sipariş alındı bilgisi ve siparişin REST API ile backende gönderilmesi ile ilgilendim. İlk 6 ay boyunca React, Gulp, SASS teknolojilerini kullandım. CSS Methodolojisi olarak BEM kullandım. 6 ay sonunda CTO'muz değişti ve tüm projenin baştan Micro ile yazmamızı ve herkesin FullStack olmasını söyledi. Bu yüzden Micro-Frontend için Qiankun kütüphanesini kullandım. Herkesin anlaması için VueJS'in daha doğru olucağına kanaat getirdik ve Nuxt ile yazdık.`,
    },
    {
      companyName: `Enuygun`,
      title: `Frontend Developer`,
      date: `05.2018 - 11.2019`,
      desc: `Enuygun'a döndüğümde Otel takımındaydım. Burada Otel projesinin önyüzünü baştan yazdım. Projede React, Webpack, SASS, Redux teknolojilerini kullandım. Otel projesini tamamladıktan sonra Test Otomasyonu yazdım. Daha sonrasında <ul><li><b>Otel:</b> Otellerin listelenmesi ve rezervasyonun oluşturulması.</li><li><b>Test Otomasyonu:</b> Yazılan kodların E2E test edilmesi.</li></ul>`,
    },
    {
      companyName: `Kolay Randevu`,
      title: `Frontend Developer`,
      date: `01.2017 - 05.2018`,
      desc: `Kolay Randevu'da sayfaların tasarımlarının revize edilmesi ile ilgilendim. Bootstrap, Grunt, SASS, Browserify teknolojilerini kullandım.`,
    },
    {
      companyName: `Enuygun`,
      title: `Junior Frontend Developer`,
      date: `07.2013 - 12.2016`,
      desc: `Frontend alanında bir eksik olduğunu görüp frontend alanına yönelmeye karar verdim. Sayfaların tasarımlarının revize edilmesi ile ilgilendim. Burada Flight Crawler ve Product Crawler adındaki iki NodeJS crawler projesini tasarladım. 2015 yılına kadar jQuery, Bootstrap, SASS, Less, Browserify teknolojilerini kullandım. 2015 yılında React ile tanıştım. Yaptığım projelerin admin panellerinde bootstrap, webpack, sass teknolojileri kullandım. 2015'den sonra React'a geçirdim. <ul><li><b>Flight Crawler:</b> Verilen sitelerdeki uçuş listesini ve detaylarını mevcut uçak biletleri ile karşılatırmayı sağlıyor.</li><li><b>Product Crawler:</b> Akakce mantığı gibi eticaret yada ürün sahibi sitelerden fiyatları çekip fiyat karşılatırmayı sağlıyor.</li></ul>`,
    },
    {
      companyName: `Enuygun`,
      title: `Stajyer`,
      date: `07.2012 - 06.2013`,
      desc: `Fullstack developer olarak çalıştım. Php, HTML ve CSS kullandım. İlk enuygun için yaptığım proje başka sitelere entegre edilebilen bir widget sistemi idi. Tüm ayarlarını url parametresi olarak alıp rengini, inputlarını vs. göster-gizle-rengini değiştir yapabiliyordu.`,
    },
  ];
</script>

<div class="experiences">
  <div class="experiences__title">Deneyimler</div>

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
      <div
        class="experience__desc"
        contenteditable
        bind:innerHTML={experience.desc}
      />
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

      & ul {
        padding-bottom: 0;
        margin-bottom: 0;
      }
    }
  }
</style>
