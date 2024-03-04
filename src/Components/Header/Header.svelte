<script>

</script>

<header class="header">
  <nav class="header__nav">
    <a href="/" class="header__nav__logo">
      Digital Financial Group
    </a>

    <div class="header__nav__links_wrapper">
      <a href="/about" class="header__nav__links_wrapper__link">About</a>
      <a href="/contacts" class="header__nav__links_wrapper__link">Contacts</a>
    </div>

  </nav>
</header>

<style lang="scss">
  @import '@/assets/styles/utils/mixins.scss';

  .header {
    display: flex;
    align-items: center;
    height: 100px;
    border-bottom: 1px groove black;
    background-color: white;
    box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(5px);

    @include mobile {
      height: 120px;
    }

    &__nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
      padding: 0 20px;
      height: 100%;

      
      @include mobile {
        padding: 0 10px;
      }

      &__logo {
        text-decoration: none;
        font-size: 40px;
        padding: 10px;
        color: rgb(0, 2, 73);
        transition: color 0.3s ease-in-out;

        @include mobile {
          font-size: 26px;
        }

        &::after {
          content: 'We purchase the solid companies and build them to last forever';
          display: block;
          margin-top: 5px;
          color: rgb(0, 2, 73);
          font-size: 14px;
          transition: color 0.3s ease-in-out;

          @include mobile {
            content: unset;
            margin-top: 0;
          }
        }

        &:hover {
          color: rgb(0, 6, 175);

          &::after {
            color: rgb(0, 6, 175);
          }
        }
      }

      &__links_wrapper {
        display: flex;
        gap: 20px;

        &__link {
          position: relative;
          text-decoration: none;
          font-size: 24px;
          padding: 20px;
          color: rgb(0, 2, 73);
          border-radius: 20px;
          transition: color 0.3s ease-in-out;

          @include mobile {
            font-size: 18px;
          }

          &::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 100%;
            height: 2px;
            background-color: transparent;
            border-radius: 10px;
            transition: background-color 0.3s ease-in-out;
          }

          &:hover {
            color: rgb(0, 6, 175);

            &::after {
              background-color: rgb(0, 6, 175);
            }
          }
        }
      }
    }
  }
</style>