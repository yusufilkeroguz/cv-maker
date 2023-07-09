<div class="educations">
  <div class="educations__title">Eğitim</div>

  <div class="education">
    Remzi Bayraktar A.T.M.L

    <div class="dates">
      <div class="date-from">2008</div>
      -
      <div class="date-to">2012</div>
    </div>
  </div>

  <div class="education">
    Sinop Üniversitesi

    <div class="dates">
      <div class="date-from">2022</div>
      -
      <div class="date-to">Current</div>
    </div>
  </div>
</div>

<style lang="scss">
  .educations {
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

    .education {
      flex: 0 0 100%;
      display: flex;
      justify-content: flex-end;
      align-items: center;
      flex-wrap: wrap;
      padding: 0.125rem;
      white-space: nowrap;

      .dates {
        flex: 0 0 100%;
        width: 100%;
        display: flex;
        justify-content: end;
        font-size: 1rem;

        .date-from {
          padding-right: 4px;
        }

        .date-to {
          padding-left: 4px;
        }
      }
    }
  }
</style>
