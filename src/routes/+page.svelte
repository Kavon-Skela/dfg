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

    <div class="main__about__text_wrapper">
      <p class="main__about__text_wrapper__text">
        We offer 24/7 access to 6000+ trained IT engineers on every continent
      </p>

      <p class="main__about__text_wrapper__text_small">
        Whether you need break fix support with critical SLA's, resource for financial projects and any other IT Services.
      </p>
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

      &__text_wrapper {
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 20px;
        width: 50%;
        height: 200px;
        padding: 20px;
        border-radius: 15px;

        @include mobile {
          width: 100%;
        }

        &__text {
          font-size: 56px;
          color: black;
          font-weight: bold;
          text-align: justify;
        }

        &__text_small {
          font-size: 32px;
          color: black;
          text-align: justify;
        }
      }
    }
  }
</style>