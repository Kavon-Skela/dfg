<script>
  import mainImg from '$lib/assets/images/main_image.webp';
</script>

<section class="main">
  <div class="main__about">
    <div class="main__about__top_section">
      <div class="main__about__top_section__block">
        <div class="main__about__top_section__block__image_wrapper">
          <img src={mainImg} alt="" class="main__about__top_section__block__image_wrapper__image">
        </div>
      </div>
    </div>

    <div class="main__about__bottom_section">
      <div class="main__about__bottom_section__block">
        <h2 class="main__about__bottom_section__block__title">
          Mission and goals
        </h2>

        <p class="main__about__bottom_section__block__text">
          Development of investment tools, fintech ecosystem and provision of access to quality financial resources to a wider client base.
        </p>
      </div>

      <div class="main__about__bottom_section__block">
        <h2 class="main__about__bottom_section__block__title">
          Own IT infrastructure
        </h2>

        <p class="main__about__bottom_section__block__text">
          A high-performance, scalable IT infrastructure ensures the security and reliability of financial processes.
        </p>
      </div>

      <div class="main__about__bottom_section__block">
        <h2 class="main__about__bottom_section__block__title">
          Security of investments
        </h2>

        <p class="main__about__bottom_section__block__text">
          The current structure of the holding ensures financial, investment, liquidity and legal stability of the group companies, as well as ensures synergy and effective implementation of new technologies.
        </p>
      </div>

      <div class="main__about__bottom_section__block">
        <h2 class="main__about__bottom_section__block__title">
          Effective management
        </h2>

        <p class="main__about__bottom_section__block__text">
          High professionalism and experience in creating effective management systems for the successful implementation of initiatives.
        </p>
      </div>
    </div>
  </div>
</section>

<style lang="scss">
  @import '@/assets/styles/utils/mixins.scss';

  .main {
    display: flex;
    align-items: center;
    padding: 0 20px;

    @include mobile {
      flex-wrap: wrap;
    }

    &__about {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 500px;
      margin: 40px auto;
      border-radius: 20px;
      gap: 40px;

      @include mobile {
        flex-direction: column;
        height: unset;
        gap: 20px;
        margin: 20px auto;
      }

      &__top_section {
        display: flex;
        justify-content: space-around;
        height: 100%;
        width: 50%;

        @include mobile {
          width: 100%;
        }

        &__block {
          width: 100%;
          height: 100%;

          &__image_wrapper {
            width: 100%;
            height: 100%;

            &__image {
              border-radius: 15px;
              width: 100%;
              height: 100%;
            }
          }
        }
      }

      &__bottom_section {
        display: flex;
        flex-direction: column;
        gap: 20px;
        width: 50%;
        height: 100%;

        @include mobile {
          width: 100%;
        }

        &__block {
          flex-basis: 25%;
          padding: 20px;
          background-color: rgba(255, 255, 255, 0.6);
          border-radius: 15px;
          
          &__title {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 10px;
            color: black;
          }

          &__text {
            font-size: 16px;
            color: black;
            text-align: justify;
          }
        }
      }
    }
  }
</style>