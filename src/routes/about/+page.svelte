<script>
  import aboutBg from '$lib/assets/images/about_bg.jpg';
</script>

<section class="about">
  <div class="about__image_wrapper">
    <img src={aboutBg} alt="" class="about__image_wrapper__image">
  </div>

  <div class="about__about">
    <span class="about__about__text">
      <strong class="about__about__text__bold">Digital Finance Group Ltd. (registration number C105643)</strong> - we are Maltese company, providing white label IT services and solutions. We send out skilled IT engineers under your brand name so you can expand your reach without employing staff directly.
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
        line-height: 140%;
        font-size: 32px;
        max-width: 600px;

        &__bold {
          font-size: 56px;

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
