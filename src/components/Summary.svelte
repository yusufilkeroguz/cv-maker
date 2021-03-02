<div class="summary">
  <div class="summary__title">
    <img src="/icons/summary.svg" alt="Summary" width={24} height="auto" />

    Summary
  </div>

  <div class="summary__content">I am Frontend Developer based on Istanbul.</div>
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
      font-size: 1.5rem;
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
