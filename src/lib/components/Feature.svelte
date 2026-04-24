<script lang="ts">
  import featureImg from "$lib/assets/Image - Everything your agent.png";
</script>

<section class="feature-section">
  <div class="feature-container">
    <!-- Left Content -->
    <div class="feature-content">
      <h2 class="feature-title">
        Everything your agent needs to go from prototype to product - fixed.
      </h2>
      <p class="feature-description">
        Modular when you want control. All-in-one when you just need to launch.
      </p>
    </div>

    <!-- Right Image -->
    <div class="feature-visual">
      <img
        src={featureImg}
        alt="Feature visual showing agent flow"
        class="feature-img"
      />
    </div>
  </div>
</section>

<style>
  .feature-section {
    width: 100%;
    background: #0a0914;
    display: flex;
    justify-content: center;
    /* padding: 60px 0; */
  }

  .feature-container {
    width: 1440px;
    height: 640px; /* From Figma layout */
    max-width: 100%;
    padding: 0 64px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .feature-content {
    width: 528px;
    display: flex;
    flex-direction: column;
    gap: 32px;
  }

  .feature-title {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1.06; /* 106% */
    letter-spacing: 0;
    color: #fafaff;
    margin: 0;
  }

  .feature-description {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 500;
    font-size: 22px;
    line-height: 1.2; /* 120% */
    letter-spacing: 0.005em; /* 0.5% */
    color: #fafaff;
    opacity: 0.74;
    margin: 0;
  }

  .feature-visual {
    width: 640px;
    height: 640px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .feature-img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  @media (max-width: 1200px) {
    .feature-container {
      flex-direction: column;
      height: auto;
      gap: 48px;
      padding: 40px 32px;
    }

    .feature-content {
      width: 100%;
      align-items: flex-start;
      text-align: left;
    }

    .feature-title {
      font-size: 32px;
    }

    .feature-description {
      font-size: 16px;
    }

    .feature-visual {
      width: 100%;
      height: auto;
    }
  }
</style>
