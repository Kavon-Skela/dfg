<section class="footer">
  <h1 class="footer__title">Contacts</h1>
  
  <article class="footer__content">
    <a target="_blank" href="https://www.google.com/maps?sca_esv=c4fb3d72123f3d0d&output=search&q=Level+G+(office+1/0991),+Quantum+House+75+Abate+Rigord+Street,+TA+XBIEX,+XBX+1120,+Malta&source=lnms&entry=mc" class="footer__content__link">Address: Level G (office 1/0991), Quantum House 75 Abate Rigord Street, TA XBIEX, XBX 1120, Malta</a>
    <a href="tel:+35622582300" class="footer__content__link">Tel.: (+356) 22582300</a>
    <a href="mailto:a.parfeniuk@garantmail.com.ua" class="footer__content__link">Email: a.parfeniuk@garantmail.com.ua</a>
  </article>
</section>

<style lang="scss">
  .footer {
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
    border-top: 1px black groove;
    box-shadow: 0 -5px 15px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(5px);

    &__title {
      font-size: 20px;
      margin-bottom: 20px;
      color: white;
    }

    &__content {
      display: flex;
      flex-direction: column;
      gap: 20px;

      &__link {
        text-decoration: none;
        font-size: 16px;
        color: white;
      }
    }
  }
</style>
