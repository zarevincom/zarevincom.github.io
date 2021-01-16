<script>
    import ButtonBase from './ButtonBase.svelte'
    import App from '../App.svelte'
</script>

<div class="app-info">
    <div class="app-info__emoji">😋</div>
    <h1 class="app-info__title ut__blockCentered">Надём место,<br>
        чтобы вкусно поесть</h1>
    <p class="app-info__descr ut__blockCentered">Вы нажимаете кнопку, а мы выдаём лучшие кафе и рестораны, с лучшими характеристиками по отзывам наших гурманов</p>
    <a href="" class="ButtonBase ButtonBase--gray ut__blockCentered">Вкусно поесть</a>
</div>

<style lang="sass">

    .ButtonBase
      display: flex
      text-align: center
      min-width: 108px
      max-width: 164px
      height: 36px
      padding: 6px 28px
      border-radius: 12px
      font-weight: 500

      &--gray
        background-color: #D8D8D8
        color: #000

    .ut__blockCentered
      margin: 0 auto
    .app-info
      display: flex
      flex-direction: column
      justify-content: space-between
      text-align: center
      margin: 0 auto

      max-width: 380px
      max-height: 248px


      &__emoji
        font-size: 48px
        margin-bottom: 12px

      &__title
        display: inline-block
        font-weight: 700
        margin-bottom: 8px
        font-size: 24px
        line-height: 28px
        max-width: 250px
        height: auto
        letter-spacing: -1.5px

      &__descr
        font-weight: 400
        font-size: 16px
        line-height: 24px
        margin-bottom: 16px
        width: 375px
</style>