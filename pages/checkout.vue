<template>
  <div class="uk-margin-large-bottom tm-checkout-page">
    <PageTitle title="Оформление заказа" />

    <section class="tm-checkout__section">
      <div class="uk-grid tm-checkout__container" uk-grid>
        <form
          class="
            uk-form-stacked uk-width-1-1 uk-width-expand@m
            tm-checkout__form
          "
          action=""
        >
          <section>
            <h2 class="tm-checkout-title">Контактная информация</h2>
            <div
              class="
                uk-card uk-card-default uk-card-small uk-card-body
                tm-checkout__fields
              "
            >
              <div
                uk-grid
                class="uk-grid-small uk-width-2-3@m uk-child-width-1-1"
              >
                <div>
                  <label>
                    <div class="uk-form-label uk-form-label-required">
                      Город получения
                    </div>
                    <input class="uk-input" type="text" required="" />
                  </label>
                </div>
                <div>
                  <label>
                    <div class="uk-form-label uk-form-label-required">
                      Имя и Фамилия по паспорту
                    </div>
                    <input class="uk-input" type="text" required="" />
                  </label>
                </div>
                <div>
                  <div
                    class="
                      uk-grid uk-grid-small
                      tm-checkout__phone-email-container
                    "
                  >
                    <label
                      class="uk-width-1-1 uk-width-2-3@s tm-checkout__email"
                    >
                      <div class="uk-form-label uk-form-label-required">
                        Email
                      </div>
                      <input class="uk-input" type="email" required="" />
                    </label>
                    <label
                      class="uk-width-1-1 uk-width-1-3@s tm-checkout__phone"
                    >
                      <div class="uk-form-label uk-form-label-required">
                        Номер телефона
                      </div>
                      <input
                        id="checkoutPhoneInput"
                        class="uk-input"
                        type="tel"
                        required=""
                      />
                    </label>
                  </div>
                </div>
              </div>
            </div>
          </section>

          <section class="uk-margin">
            <h2 class="tm-checkout-title">Способ получения</h2>
            <div
              class="
                uk-card uk-card-default uk-card-small uk-card-body
                tm-checkout__fields
              "
            >
              <ul
                class="
                  uk-flex-between uk-subnav uk-subnav-pill
                  tm-checkout__receive-method-tab
                "
                uk-tab="animation: uk-animation-fade"
              >
                <li>
                  <a href="#"> Самовывоз </a>
                </li>
                <li>
                  <a href="#"> Доставка курьером </a>
                </li>
                <li>
                  <a href="#"> Доставка почтой </a>
                </li>
              </ul>
              <ul class="uk-switcher uk-margin">
                <li>
                  <div class="uk-grid">
                    <div class="uk-width-1-1 uk-width-2-3@s">
                      <iframe
                        src="https://yandex.ru/map-widget/v1/?um=constructor%3Aa20928f0cbee1fc6d57e819478c4c1e68a2b3934ee2a0b33b987b664b9754d4b&amp;source=constructor"
                        width="100%"
                        height="300"
                        frameborder="0"
                      ></iframe>
                    </div>
                    <div class="uk-width-1-1 uk-width-1-3@s">
                      <h3>Название магазина</h3>
                      <p>Москва, Красная площадь, 3, второй этаж</p>
                      <p>Ежедневно с 10:00 до 22:00</p>
                    </div>
                  </div>
                </li>
                <li>
                  <h3 class="uk-margin-bottom">Адрес получения</h3>

                  <div class="uk-grid uk-grid-small">
                    <div class="uk-width-1-1 uk-width-2-3@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Улица
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div class="uk-width-1-1 uk-width-1-3@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Дом
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                  </div>
                  <div
                    class="
                      uk-grid
                      uk-grid-small
                      uk-child-width-1-2
                      uk-child-width-1-4@s
                    "
                  >
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Строение
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Подъезд
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Этаж
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Квартира
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                  </div>
                  <div class="uk-width-1-1 tm-checkout__comment-block">
                    <label>
                      <div class="uk-form-label">Комментарий</div>
                      <textarea
                        class="uk-textarea"
                        rows="5"
                        placeholder="Дополнительная информация к заказу"
                      ></textarea>
                    </label>
                  </div>
                  <div
                    class="
                      uk-grid-small
                      uk-child-width-1-2
                      uk-child-width-1-4@s
                      uk-grid
                      tm-checkout__delivery-date-time
                    "
                    uk-grid=""
                  >
                    <div class="uk-width-1-1 uk-form-label">
                      Дата и время доставки
                    </div>
                    <div class="uk-margin-remove uk-first-column">
                      <select class="uk-select">
                        <option>Завтра</option>
                        <option>27 января</option>
                        <option>28 января</option>
                        <option>29 января</option>
                        <option>30 января</option>
                        <option>31 января</option>
                        <option>1 февраля</option>
                      </select>
                    </div>
                    <div class="uk-margin-remove">
                      <select class="uk-select">
                        <option>09:00 – 12:00</option>
                        <option>12:00 – 15:00</option>
                        <option>15:00 – 18:00</option>
                        <option>18:00 – 21:00</option>
                        <option>21:00 – 23:00</option>
                      </select>
                    </div>
                  </div>
                </li>
                <li>
                  <h3 class="uk-margin-bottom">Адрес получения</h3>

                  <div class="uk-grid uk-grid-small">
                    <div class="uk-width-1-1 uk-width-3-4@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Город
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div class="uk-width-1-1 uk-width-1-4@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Почтовый индекс
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                  </div>
                  <div class="uk-grid uk-grid-small">
                    <div class="uk-width-1-1 uk-width-2-3@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Улица
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div class="uk-width-1-1 uk-width-1-3@s">
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Дом
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                  </div>
                  <div
                    class="
                      uk-grid
                      uk-grid-small
                      uk-child-width-1-2
                      uk-child-width-1-4@s
                    "
                  >
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Строение
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Подъезд
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Этаж
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                    <div>
                      <label>
                        <div class="uk-form-label uk-form-label-required">
                          Квартира
                        </div>
                        <input class="uk-input" type="text" required="" />
                      </label>
                    </div>
                  </div>
                  <div class="uk-width-1-1 tm-checkout__comment-block">
                    <label>
                      <div class="uk-form-label">Комментарий</div>
                      <textarea
                        class="uk-textarea"
                        rows="5"
                        placeholder="Дополнительная информация к заказу"
                      ></textarea>
                    </label>
                  </div>
                </li>
              </ul>
            </div>
          </section>

          <section class="uk-margin-top">
            <h2 class="tm-checkout-title">Способ оплаты</h2>
            <div class="uk-card uk-card-default uk-card-small">
              <div class="uk-card-body">
                <ul
                  class="
                    uk-subnav
                    uk-subnav-pill
                    uk-grid-small
                    uk-grid-match
                    uk-child-width-1-1
                    uk-child-width-1-3@s
                    uk-flex-center
                    uk-grid
                  "
                  uk-switcher
                  uk-grid
                >
                  <li>
                    <a class="tm-checkout__payment-choice" href="#">
                      Картой онлайн
                    </a>
                  </li>
                  <li>
                    <a class="tm-checkout__payment-choice" href="#"> Картой </a>
                  </li>
                  <li>
                    <a class="tm-checkout__payment-choice" href="#">
                      Наличными
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </section>
        </form>

        <div class="uk-width-1-1 uk-width-1-4@m tm-checkout__sticky-cart">
          <div
            class="uk-card uk-card-default uk-card-small uk-sticky"
            uk-sticky="offset: 90; bottom: true; media: @m;"
            style=""
          >
            <section class="uk-card-body">
              <h4>Товары в корзине</h4>
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-small">
                    Nike Air Force 1 Mid (<span>Белый</span>)
                  </div>
                  <div class="uk-text-meta">1 × 7999 ₽</div>
                </div>
                <div class="uk-text-right">
                  <div>7999 ₽</div>
                </div>
              </div>
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-small">
                    Носки Best Socks (Белый, Серый, Чёрный)
                  </div>
                  <div class="uk-text-meta">2 × 798 ₽</div>
                </div>
                <div class="uk-text-right">
                  <div>399 ₽</div>
                </div>
              </div>
            </section>
            <section class="uk-card-body">
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-muted">Доставка</div>
                </div>
                <div class="uk-text-right">
                  <div>Самовывоз</div>
                  <div class="uk-text-meta">Бесплатно, сегодня</div>
                </div>
              </div>
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-muted">Оплата</div>
                </div>
                <div class="uk-text-right">
                  <div>Картой онлайн</div>
                </div>
              </div>
            </section>
            <section class="uk-card-body">
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-muted">Подитог</div>
                </div>
                <div class="uk-text-right">
                  <div>8797 ₽</div>
                </div>
              </div>
              <div class="uk-grid-small uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-muted">Скидка</div>
                </div>
                <div class="uk-text-right">
                  <div class="uk-text-danger">− 798 ₽</div>
                </div>
              </div>
            </section>
            <section class="uk-card-body">
              <div class="uk-grid-small uk-flex-middle uk-grid" uk-grid="">
                <div class="uk-width-expand uk-first-column">
                  <div class="uk-text-muted">Итого</div>
                </div>
                <div class="uk-text-right">
                  <div class="uk-text-lead uk-text-bolder">7999 ₽</div>
                </div>
              </div>
              <button
                class="
                  uk-button
                  uk-button-primary
                  uk-button-large
                  uk-border-pill
                  uk-margin
                  uk-width-1-1
                  tm-checkout__pay-btn
                "
              >
                Перейти к оплате
              </button>
            </section>
          </div>
          <div
            class="uk-sticky-placeholder"
            style="height: 620px; margin: 0px"
            hidden=""
          ></div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import PageTitle from '@/components/PageTitle'

export default {
  name: 'CheckoutPage',

  components: {
    PageTitle
  }
}
</script>

<style lang="scss" scoped>
.tm-checkout {
  &__section {
    max-width: 1100px;
    margin: 0 auto;
  }
  &__container {
  }
  &__form {
    // margin-left: 0;
  }
  &__sticky-cart {
    margin: 56px 0 0 0;
    z-index: 1;
  }

  &__receive-method-tab a[aria-expanded='true'] {
    background-color: #1e87f0 !important;
    color: #fff !important;
  }

  &__comment-block,
  &__delivery-date-time {
    margin-top: 15px;
  }

  &__payment-choice {
    height: 40px;
    line-height: 30px;
    text-align: center;
    border-radius: 4px;
  }

  &__pay-btn {
    // line-height: 38px;
  }
}

//@media (max-width: 1100px) {
//  .tm-checkout {
//    &__sticky-cart {
//      max-width: 500px;
//      margin: 56px auto 0;
//    }
//    &__pay-btn {
//      padding: 0 15px;
//      line-height: 38px;
//    }
//  }
//}
//
//@media (max-width: 960px) {
//  .tm-checkout {
//    &__fields > div {
//      margin-left: 0 !important;
//    }
//  }
//}
//
//@media (max-width: @xsm) {
//  .tm-checkout {
//    &__email {
//      margin-bottom: 15px;
//    }
//  }
//}
</style>
