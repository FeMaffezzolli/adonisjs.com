<template>
  <section class="video">
    <div class="container">
      <div class="video-container">

        <SectionTitle theme="light"> AdonisJS v5 tour </SectionTitle>

        <SectionSubTitle theme="light">
          Let's take a tour of AdonisJS together. The screencast will not make you the framework expert, but instead it serves as a great building block before moving forward.
        </SectionSubTitle>

        <div class="embed-player" ref="embed-player">
          <div class="embed-container">
            <iframe class="embed" src="https://www.youtube.com/embed/TysfaNcFX_Y" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  import SectionTitle from '~/components/SectionTitle'
  import SectionSubTitle from '~/components/SectionSubTitle'

  export default {
    components: { SectionSubTitle, SectionTitle },
  }
</script>

<style scoped>
  .video {
    background: var(--brand);
    background-image: linear-gradient(180deg, var(--brand) 0%, #4434BF 100%);
  }

  .label {
    background: #FFFFFF;
    border-radius: 2px;
    font-weight: 600;
    font-family: var(--font-secondary);
    padding: 10px 15px;
    display: inline-block;
    font-size: 1.3rem;
    color: var(--brand);
    letter-spacing: 1.2px;
    text-transform: uppercase;
  }

  .video-container {
    padding-top: 100px;
  }

  .embed-player {
    margin-top: 40px;
    background: var(--pre-bg);
    font-size: 2.5rem;
    font-family: var(--font-mono);
    color: #7a7b90;
    z-index: 1;
    position: relative;
    padding-bottom: 56.25%;
    border-radius: 4px;
  }

  .embed-container .embed {
    position: absolute;
    top: 0;
    left: 0;
    padding: 8px;
    width: 100%;
    height: 100%;
  }

  @media (min-width: 768px) {
    .video-container {
      max-width: 600px;
      text-align: center;
      margin: auto;
    }
  }

  @media (min-width: 1024px) {
    .video-container {
      max-width: 800px;
      padding-top: 100px;
    }

    .video-container .subtitle {
      padding: 0 70px;
    }
  }
</style>
