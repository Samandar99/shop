<template>
  <nav class="header" :class="{ actives: !openMenu }">
    <div class="news">
      <div class="news-left">
        <img src="@/assets/images/Icon.svg" alt="" />
        <span>Москва</span>
      </div>
      <div class="news-right">
        <ul class="news__list">
          <li>Бренды</li>
          <li>Доставка</li>
          <li>Возврат</li>
          <li>Документация</li>
          <li>Контакты</li>
        </ul>
      </div>
    </div>
    <div class="draw">
      <div class="header-search">
        <div class="header-search__left">
          <img src="@/assets/images/Vector.svg" alt="" />
          <span>StroykaStore</span>
        </div>
        <div class="header-search__right">
          <div class="search-categories">
            <div class="catalog">
              <img
                class="catalog-icon"
                src="@/assets/images/katalog.svg"
                alt=""
              />
              <span>Каталог</span>
            </div>
            <div class="search__input">
              <input type="text" />
              <img src="@/assets/images/searchIcon.svg" alt="" />
            </div>
            <div class="icons">
              <div class="icon-person">
                <img src="@/assets/images/person.svg" alt="" />
                <span>Профиль</span>
              </div>
              <div class="icon-person">
                <img src="@/assets/images/Icon1.svg" alt="" />
                <span>Заказы</span>
              </div>
              <div class="icon-person">
                <img src="@/assets/images/Icon2.svg" alt="" />
                <span>Корзина</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="close_icon" @click="openMenu = !openMenu">
      <i class="fa fa-times fa-2x" v-if="openMenu"></i>
      <i class="fa-solid fa-bars fa-2x" v-else></i>
    </div>
  </nav>

  <Swiper
    class="swiperBaner"
    :modules="modules"
    :space-between="20"
    :loop="true"
    :navigation="{
      prevEl: prev,
      nextEl: next,
    }"
    :autoplay="{
      delay: 4000,
      disableOnInteraction: false,
      pauseOnMouseEnter: true,
    }"
  >
    <swiper-slide>
      <div class="bannerFoto">
        <div class="banner">
          <div class="banner-left">
            <h1>Специальные предложения</h1>
            <p>
              «СтройкаСтор» стремится сделать условия покупки максимально
              выгодными для каждого покупателя, поэтому на сайте регулярно
              появляются товары со скидкой
            </p>
            <button>Подробнее</button>
          </div>
        </div>
      </div>
    </swiper-slide>

    <swiper-slide>
      <div class="bannerFoto1">
        <div class="banner1">
          <div class="banner-left2">
            <h1>Распродажа инструментов</h1>
            <p>на строительные материалы и товары для ремонта</p>
            <button>Подробнее</button>
          </div>
        </div>
      </div>
    </swiper-slide>

    <swiper-slide>
      <div class="bannerFoto">
        <div class="banner">
          <div class="banner-left">
            <h1>Специальные предложения</h1>

            <p>
              «СтройкаСтор» стремится сделать условия покупки максимально
              выгодными для каждого покупателя, поэтому на сайте регулярно
              появляются товары со скидкой
            </p>
            <button>Подробнее</button>
          </div>
        </div>
      </div>
    </swiper-slide>

    <div class="arrow">
      <div ref="prev" class="swiper">
        <div class="put">
          <img src="@/assets/images/arrowLeft.svg" alt="" />
        </div>
      </div>
      <div ref="next" class="swiper">
        <div class="put">
          <img src="@/assets/images/arrowRight.svg" alt="" />
        </div>
      </div>
    </div>
  </Swiper>

  <section class="container-Discount">
    <div class="discount__header">
      <h3 class="discount__header-title">Акции</h3>
      <div class="dis-btn">
        <span>Все акции</span>
        <img src="@/assets/images/arrwoRighta.svg" alt="" />
      </div>
    </div>
    <div class="block-discount__products">
      <div class="discount__prouducts-left">
        <div class="main-left">
          <div class="skidkas">
            <span>−25%</span>
          </div>
          <img
            class="products__img-discount"
            src="@/assets/images/Image.png"
            alt=""
          />
        </div>
        <div class="main-right">
          <p>Рубероид РКП-350 ТУ, размер материала 1 х 10 м (10м2, 1 рулон)</p>

          <div>
            <div class="price__products">
              <h3>449 ₽</h3>
              <span class="sale">523 ₽</span>
            </div>
            <button class="products_btn">В корзину</button>
          </div>
        </div>
      </div>
      <div class="discount__prouducts-left">
        <div class="main-left">
          <div class="skidkas">
            <span>−25%</span>
          </div>
          <img
            class="products__img-discount"
            src="@/assets/images/Image3.png"
            alt=""
          />
        </div>
        <div class="main-right">
          <p>Рубероид РКП-350 ТУ, размер материала 1 х 10 м (10м2, 1 рулон)</p>

          <div>
            <div class="price__products">
              <h3>449 ₽</h3>
              <span class="sale">523 ₽</span>
            </div>
            <button class="products_btn">В корзину</button>
          </div>
        </div>
      </div>
      <div class="discount__prouducts-left">
        <div class="main-left">
          <div class="skidkas">
            <span>−25%</span>
          </div>
          <img
            class="products__img-discount"
            src="@/assets/images/Image5.png"
            alt=""
          />
        </div>
        <div class="main-right">
          <p>Рубероид РКП-350 ТУ, размер материала 1 х 10 м (10м2, 1 рулон)</p>

          <div>
            <div class="price__products">
              <h3>449 ₽</h3>
              <span class="sale">523 ₽</span>
            </div>
            <button class="products_btn">В корзину</button>
          </div>
        </div>
      </div>
      <div class="discount__prouducts-left">
        <div class="main-left">
          <div class="skidkas">
            <span>−25%</span>
          </div>
          <img
            class="products__img-discount"
            src="@/assets/images/Image6.png"
            alt=""
          />
        </div>
        <div class="main-right">
          <p>Рубероид РКП-350 ТУ, размер материала 1 х 10 м (10м2, 1 рулон)</p>

          <div>
            <div class="price__products">
              <h3>449 ₽</h3>
              <span class="sale">523 ₽</span>
            </div>
            <button class="products_btn">В корзину</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="categories">
    <div class="categories__header">
      <h3 class="discount__header-title">Популярные категории</h3>
      <div class="dis-btn">
        <span>Все категории</span>
        <img src="@/assets/images/arrwoRighta.svg" alt="" />
      </div>
    </div>
    <div class="blocks">
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image48.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image49.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image53.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image54.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image55.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image56.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image86.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image87.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image88.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image89.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/image90.png" alt="" />
      </div>
      <div class="box__categories">
        <p>Пиломатериалы</p>
        <img src="@/assets/imagesCategories/pngwing1.png" alt="" />
      </div>
    </div>
  </section>

  <section class="famous__products">
    <h3 class="famous-title">Популярные товары</h3>
    <div class="block-famous">
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image3.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image5.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image6.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image7.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image8.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image9.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image10.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image11.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image12.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image13.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image14.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
      <div class="box-famous">
        <div class="famus_img">
          <img src="@/assets/images/Image15.png" alt="" />
        </div>

        <div class="gon">
          <p>Керамогранит Yasmin 598х185 коричневый C-YA4M112D</p>
          <b class="price">899 ₽</b>
          <button class="famous-btn">В корзину</button>
        </div>
      </div>
    </div>
  </section>

  <section class="popular__brands">
    <div class="categories__header mt">
      <h3 class="discount__header-title">Популярные бренды</h3>
      <div class="dis-btn">
        <span>Все категории</span>
        <img src="@/assets/images/arrwoRighta.svg" alt="" />
      </div>
    </div>
    <div class="popular__container">
      <div class="popular__box">
        <img src="@/assets/images/image60.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image65.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image62.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image63.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image64.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image65.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image66.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image67.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image68.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image69.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image70.png" alt="" />
      </div>
      <div class="popular__box">
        <img src="@/assets/images/image71.png" alt="" />
      </div>
    </div>
  </section>
  <section class="users-container">
    <div class="head-users">
      <h3 class="user-title">Отзывы</h3>
      <div class="arrow2">
        <div ref="prev1" class="swiper">
          <div class="put">
            <img src="@/assets/images/arrowLeft.svg" alt="" />
          </div>
        </div>
        <div ref="next1" class="swiper">
          <div class="put">
            <img src="@/assets/images/arrowRight.svg" alt="" />
          </div>
        </div>
      </div>
    </div>

    <Swiper
      :slidesPerView="3"
      :spaceBetween="30"
      :modules="modules"
      :navigation="{
        prevEl: prev1,
        nextEl: next1,
      }"
      class="mySwiper"
    >
      <swiper-slide class="carusel__box1">
        <div class="carusel__box">
          <div class="head">
            <div class="head-name">
              <img src="@/assets/images/Avatars(2).svg" alt="" />
              <span>Пётр</span>
            </div>

            <img src="@/assets/images/image84(Traced).svg" alt="" />
          </div>

          <p class="text-users">
            Сегодня 10.03.2022 года, брал перфоратор в аренду в магазине по
            улице Дорожная. Продавец всё хорошо объяснил, показал и плюс остался
            бонус в ящике перфоратора это бур нужного мне диаметра, оставленным
            прежним арендатором. В общем повесил телевизор, где надо было
            просверлить 4 отверстия, всего за 100 ₽
          </p>
          <span class="date-user"> 21 марта 2022 г. </span>
        </div>
      </swiper-slide>
      <swiper-slide class="carusel__box1">
        <div class="carusel__box">
          <div class="head">
            <div class="head-name">
              <img src="@/assets/images/Avatars(1).svg" alt="" />
              <span>Анна</span>
            </div>

            <img src="@/assets/images/image84(Traced).svg" alt="" />
          </div>

          <p class="text-users">
            Сегодня 10.03.2022 года, брал перфоратор в аренду в магазине по
            улице Дорожная. Продавец всё хорошо объяснил, показал и плюс остался
            бонус в ящике перфоратора это бур нужного мне диаметра, оставленным
            прежним арендатором. В общем повесил телевизор, где надо было
            просверлить 4 отверстия, всего за 100 ₽
          </p>
          <span class="date-user"> 21 марта 2022 г. </span>
        </div></swiper-slide
      >
      <swiper-slide class="carusel__box1">
        <div class="carusel__box">
          <div class="head">
            <div class="head-name">
              <img src="@/assets/images/Avatars(3).svg" alt="" />
              <span>Виктор</span>
            </div>

            <img src="@/assets/images/image84(Traced).svg" alt="" />
          </div>

          <p class="text-users">
            Сегодня 10.03.2022 года, брал перфоратор в аренду в магазине по
            улице Дорожная. Продавец всё хорошо объяснил, показал и плюс остался
            бонус в ящике перфоратора это бур нужного мне диаметра, оставленным
            прежним арендатором. В общем повесил телевизор, где надо было
            просверлить 4 отверстия, всего за 100 ₽
          </p>
          <span class="date-user"> 21 марта 2022 г. </span>
        </div></swiper-slide
      >
      <swiper-slide class="carusel__box1">
        <div class="carusel__box">
          <div class="head">
            <div class="head-name">
              <img src="@/assets/images/Avatars(4).svg" alt="" />
              <span>Дмитрий</span>
            </div>

            <img src="@/assets/images/image84(Traced).svg" alt="" />
          </div>

          <p class="text-users">
            Сегодня 10.03.2022 года, брал перфоратор в аренду в магазине по
            улице Дорожная. Продавец всё хорошо объяснил, показал и плюс остался
            бонус в ящике перфоратора это бур нужного мне диаметра, оставленным
            прежним арендатором. В общем повесил телевизор, где надо было
            просверлить 4 отверстия, всего за 100 ₽
          </p>
          <span class="date-user"> 21 марта 2022 г. </span>
        </div></swiper-slide
      >
      <swiper-slide class="carusel__box1">
        <div class="carusel__box">
          <div class="head">
            <div class="head-name">
              <img src="@/assets/images/Avatars(1).svg" alt="" />
              <span>Пётр</span>
            </div>

            <img src="@/assets/images/image84(Traced).svg" alt="" />
          </div>

          <p class="text-users">
            Сегодня 10.03.2022 года, брал перфоратор в аренду в магазине по
            улице Дорожная. Продавец всё хорошо объяснил, показал и плюс остался
            бонус в ящике перфоратора это бур нужного мне диаметра, оставленным
            прежним арендатором. В общем повесил телевизор, где надо было
            просверлить 4 отверстия, всего за 100 ₽
          </p>
          <span class="date-user"> 21 марта 2022 г. </span>
        </div>
      </swiper-slide>
    </Swiper>
  </section>

  <section class="about__company">
    <div class="about-text">
      <h3>О компании</h3>
      <p>
        В СтройкаСтор вы всегда можете купить все необходимые товары для ремонта
        домаи дачи. Хотите сделать ремонт в квартире? Строите загородный дом?
        Используйте строительные и отделочные материалы из нашего каталога.
      </p>
      <p class="aboutWords">
        Быстрая доставка строительных товаров по низким ценам сделает ваши
        покупки более приятными. Ремонт может стоить дешево, если делать его с
        нами. Для вас всегда в наличии более 30 000 товаров для строительства по
        низким ценам каждый день. СтройкаСтор — это широкий ассортимент товаров
        для дома и ремонта недорого; Возможность заказать строительные и
        отделочные материалы для дома и дачи.
      </p>
    </div>
  </section>

  <section class="footer">
    <div class="main__footer">
      <div class="footer-box">
        <ul class="main__list1">
          <li class="listfooter">
            <img src="@/assets/images/Vector.svg" alt="" />
            <span> StroykaStore </span>
          </li>
          <li class="listfooter1">
            <img src="@/assets/images/message.svg" alt="" />
            <span> info@stroykastore.ru </span>
          </li>
          <li class="listfooter2">
            <img src="@/assets/images/location.svg" alt="" />
            <span> Москва, ул. Камушкина 10</span>
          </li>
        </ul>
        <ul class="main-list">
          <li class="listfooter">
            <span> Личный кабинет </span>
          </li>
          <li class="listfooter">
            <span> Заказы </span>
          </li>
          <li class="listfooter">
            <span>Избранное</span>
          </li>
          <li class="listfooter">
            <span>Корзина</span>
          </li>
        </ul>
        <ul class="main-list">
          <li class="listfooter">
            <span> Каталог </span>
          </li>
          <li class="listfooter">
            <span> Акции </span>
          </li>
          <li class="listfooter">
            <span>Бренды</span>
          </li>
          <li class="listfooter">
            <span>Контакты</span>
          </li>
        </ul>
        <ul class="main-list">
          <li class="listfooter">
            <span> Стать продавцом </span>
          </li>
          <li class="listfooter">
            <span> Доставка </span>
          </li>
          <li class="listfooter">
            <span>Возврат</span>
          </li>
          <li class="listfooter">
            <span>Документация</span>
          </li>
        </ul>
      </div>
    </div>
    <div class="footer-send">
      <div>
        <span>© СтройкаСтор</span>
      </div>
      <div class="footer__icons">
        <img src="@/assets/images/Visacart.svg" alt="" />
        <img src="@/assets/images/visa.svg" alt="" />
        <img src="@/assets/images/visa2.svg" alt="" />
        <img src="@/assets/images/mir.svg" alt="" />
      </div>
      <div>
        <span>Cделано в KRUGLOV STUDIO</span>
      </div>
    </div>
  </section>

  <!-- <router-link to="/">Дом</router-link> |
  <router-link to="/about">О нас</router-link>

  <router-view /> -->
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay, Pagination } from "swiper";
import { ref } from "vue";
import { Navigation } from "swiper";

import "swiper/css/navigation";
import "swiper/css";
import "swiper/css/pagination";

import "@/assets/style/header.css";
import "@/assets/style/discount.css";
import "@/assets/style/categories.css";
import "@/assets/style/famous.css";
import "@/assets/style/footer.css";
export default {
  components: { Swiper, SwiperSlide },

  data() {
    return {
      openMenu: true,
    };
  },

  setup() {
    const prev = ref(null);
    const next = ref(null);
    const prev1 = ref(null);
    const next1 = ref(null);
    return {
      modules: [Pagination, Autoplay, Navigation],
      prev,
      next,
      prev1,
      next1,
    };
  },
};
</script>

<style scoped>
a.router-link-exact-active {
  color: #42b983;
}
</style>
