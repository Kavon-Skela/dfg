<script>
  import aboutBg from '$lib/assets/images/about_bg.jpg';
</script>

<section class="about">
  <div class="about__image_wrapper">
    <img src={aboutBg} alt="" class="about__image_wrapper__image">
  </div>

  <div class="about__about">
    <span class="about__about__text">
      <strong class="about__about__text__bold">Digital Finance Group Ltd. (registration number C105643)</strong> - is a Maltese company,  investing in business projects throughout the EU.
      We are a long-term holding company dedicated to buying and building successful businesses and managing them with exceptional, values-based leadership.
      The main object of our company is to subcribe of any shares of any entity in the name of and on behalf of the company.
    </span>
  </div>
</section>

<style lang="scss">
  @import '@/assets/styles/utils/mixins.scss';

  .about {
    display: flex;
    gap: 60px;
    padding: 50px;
    margin: 60px auto;

    @include mobile {
      flex-wrap: wrap;
      padding: 20px;
      margin: 0 auto;
      gap: 20px;
    }

    &__about {
      &__text {
        display: block;
        color: black;
        text-align: justify;
        line-height: 140%;
        font-size: 18px;
        max-width: 600px;

        &__bold {
          font-size: 28px;

          @include mobile {
            font-size: 24px;
          }
        }
      }
    }

    &__image_wrapper {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      max-width: 600px;
      height: 100%;
      border-radius: 20px;

      &__image {
        width: 600px;
        max-width: 600px;
        height: 100%;
        object-fit: cover;
        border-radius: 20px;

        @include mobile {
          width: 100%;
        }
      }
    }
  }
</style>
