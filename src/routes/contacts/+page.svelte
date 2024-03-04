<script>
  import contactsBG from '$lib/assets/images/contacts_bg.jpg';
</script>

<section class="contacts">
  <div class="contacts__wrapper">
    <div class="contacts__image_wrapper">
      <img src={contactsBG} alt="" class="contacts__image">
    </div>

    <article class="contacts__content">
      <a target="_blank" href="https://www.google.com/maps?sca_esv=c4fb3d72123f3d0d&output=search&q=Level+G+(office+1/0991),+Quantum+House+75+Abate+Rigord+Street,+TA+XBIEX,+XBX+1120,+Malta&source=lnms&entry=mc" class="contacts__content__link">Address: Level G (office 1/0991), Quantum House 75 Abate Rigord Street,</a>
      <a target="_blank" href="https://www.google.com/maps?sca_esv=c4fb3d72123f3d0d&output=search&q=Level+G+(office+1/0991),+Quantum+House+75+Abate+Rigord+Street,+TA+XBIEX,+XBX+1120,+Malta&source=lnms&entry=mc" class="contacts__content__link">TA XBIEX, XBX 1120, Malta</a>
      <a href="tel:+35622582300" class="contacts__content__link">Tel.: (+356) 22582300</a>
      <a href="mailto:a.parfeniuk@garantmail.com.ua" class="contacts__content__link">Email: a.parfeniuk@garantmail.com.ua</a>
    </article>
  </div>
  

</section>

<style lang="scss">
  @import '@/assets/styles/utils/mixins.scss';

  .contacts {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 50px;

    @include mobile {
      padding: 20px;
    }

    &__wrapper {
      display: flex;
      gap: 20px;
      margin-top: 60px;

      @include mobile {
        flex-wrap: wrap;
        margin-top: 0;
      }
    }

    &__image_wrapper {
      width: 100%;
      max-width: 600px;
      height: 100%;
      border-radius: 20px;
    }

    &__image {
      width: 100%;
      max-width: 600px;
      height: 100%;
      object-fit: cover;
      border-radius: 20px;
    }

    &__content {
      display: flex;
      flex-direction: column;
      justify-content: end;
      gap: 20px;

      &__link {
        text-decoration: none;
        font-size: 18px;
        color: black;
      }
    }
  }
</style>
