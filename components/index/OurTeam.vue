<template>
  <div class="c-our-team">
    <div class="c-our-team__content">
      <div class="c-our-team__photo">
        <img src="https://picsum.photos/484/242" />
      </div>
      <div class="c-our-team__text">
        <h1 class="c-our-team__header">{{ $t('Our team & history') }}</h1>
        <p>{{ $t('We\’re a 6 year old foundation with amazing growth and many twists and turns on the way.') }}</p>
        <a href="#">{{ $t('Find Out More') }}</a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import '~/assets/_variables.scss';

  .c-our-team {
    background: $grey-bg;
    padding: 40px 0;

    &__content {
      max-width: $content-width;
      margin: 40px auto;
      display: flex;
    }

    &__photo {
      flex: 1;
      margin-right: 20px;

      img {
        width: 100%;
      }
    }

    &__text {
      flex: 1;
      display: flex;
      flex-direction: column;
      margin-left: 20px;

      p {
        flex: 1;
        margin: 10px 0;
      }

      a {
        color: $cd-orange;
        margin: 25px 0;
        font-size: 18px;
        font-weight: bold;
      }
    }

    &__header {
      margin-top: 0;
      text-align: left;
    }
  }

  @include media-breakpoint-max(sm) {
    .c-our-team {
      &__content {
        flex-direction: column-reverse;
      }

      &__photo {
        margin: 0;
      }

      &__text {
        margin: 0 20px;
      }
    }
  }
</style>
