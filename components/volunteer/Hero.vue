<template>
  <div class="c-hero">
    <h1 class="c-hero__header1">{{ $t('Volunteer at a Dojo near you') }}</h1>
    <div class="c-hero__images">
      <div class="c-hero__image">
        <img src="https://picsum.photos/480/320?image=1" />
      </div>
      <div class="c-hero__image">
        <img src="https://picsum.photos/480/320?image=2" />
      </div>
      <div class="c-hero__image">
        <img src="https://picsum.photos/480/320?image=3" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import '~/assets/_variables.scss';

  .c-hero {
    padding: 0 0 80px 0;
    background-image:
      linear-gradient(to bottom, $cd-purple 0%, $cd-purple-gradient 100%);

    &__header1 {
      color: $white;
      font-weight: 300;
      font-size: 40px;
      max-width: 900px;
      margin: 0 auto;
      padding: 50px 20px;
    }

    &__images {
      display: flex;
      max-width: $content-width;
      margin: 30px auto 0 auto;
    }

    &__image {
      flex: 1;
      justify-content: space-between;
      margin: 0 20px;

      img {
        width: 100%;
      }
    }
  }

  @include media-breakpoint-max(sm) {
    .c-hero {
      background-image:
        linear-gradient(to bottom, $cd-purple 0%, $cd-purple-gradient 100%);

      &__header1 {
        font-size: 22px;
      }

      &__header2 {
        font-size: 12px;
      }

      &__images {
        flex-direction: column;
      }

      &__image {
        margin: 20px 40px;

        &:first-child {
          display: none;
        }
      }
    }
  }
</style>
