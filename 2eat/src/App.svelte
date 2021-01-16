<script>
    import AppInfo from './components/AppInfo.svelte'
    import ButtonBase from './components/ButtonBase.svelte'
    import AppMap from './components/AppMap.svelte'

    let ifInfoAvailable = true
    let marginBottom = ifInfoAvailable === true ? 'mbToSection' : 'mbToMap'
</script>

<main class="main-content" id="app">
    <div class="container">
        <header class="{marginBottom}">
            <nav class="navigation">
                <div class="nav-logo">
                    <div class="nav-logo__img"><img src="/assets/imgs/storefront.svg" alt="2Eat logo - an icon of a store"></div>
                    <div class="nav-logo__text">2Eat</div>
                </div>
                <ButtonBase>Войти</ButtonBase>
            </nav>
        </header>
        {#if ifInfoAvailable}
            <AppInfo></AppInfo>
        {:else}
            <AppMap></AppMap>
        {/if}
    </div>
</main>

<style type="text/sass">
    .mbToSection
      margin-bottom: 295px
    .mbToMap
      margin-bottom: 40px
    body

      font-family: 'TT Norms'
    .container
      width: 80%
      margin: 0 auto

    .navigation
      min-width: 72px
      display: flex
      align-content: center
      justify-content: space-between
      padding: 20px 0

    .nav-logo
      display: flex
      align-content: center
      justify-content: space-between
      max-width: 100px
      &__text
        font-size: 26px
        line-height: 31px
        color: #000
        margin-left: 10px
        font-weight: 500





</style>