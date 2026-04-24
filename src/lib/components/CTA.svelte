<script lang="ts">
  import ctaIcon from '$lib/assets/Group 758531964.png';
  import ctaPlanet from '$lib/assets/Plannet-Violet.png';
  import ctaGlow from '$lib/assets/Ellipse 385.png';
</script>

<section class="cta-section">
  <!-- The glowing planet background -->
  <div class="planet-bg">
    <img src={ctaGlow} alt="Glow" class="glow-img" />
    <img src={ctaPlanet} alt="Planet glow" class="planet-img" />
  </div>

  <div class="cta-container">
    <div class="cta-icon-wrapper">
      <img src={ctaIcon} alt="CometChat Icon" class="cta-icon" />
    </div>

    <div class="cta-text-content">
      <h2 class="cta-title">You don't need to build it<br/>all to ship it all</h2>
      <p class="cta-subtitle">
        Start with chat. Or go full stack. Build fast, scale securely, and<br/>
        focus on what your agent does - not what it's missing.
      </p>
    </div>

    <div class="cta-actions">
      <button class="btn-ghost">Talk to Us</button>
      <button class="btn-primary">Try the Agent Builder</button>
    </div>
  </div>
</section>

<style>
  .cta-section {
    width: 100%;
    background: #0A0914;
    display: flex;
    justify-content: center;
    position: relative;
    overflow: hidden; 
    min-height: 647px; /* Based on Figma section height */
  }

  .planet-bg {
    position: absolute;
    top: 221px; 
    left: 50%;
    transform: translateX(-50%);
    width: 1434px;
    height: 1434px;
    z-index: 1;
    pointer-events: none;
    display: flex;
    justify-content: center;
  }

  .glow-img {
    position: absolute;
    top: -100px;
    width: 642px;
    height: 400px;
    opacity: 0.6;
    z-index: 1;
  }

  .planet-img {
    position: relative;
    width: 100%;
    height: 100%;
    object-fit: contain;
    z-index: 2;
  }

  .cta-container {
    position: relative;
    z-index: 2;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    max-width: 1440px;
    padding-top: 40px; /* Figma: Icon is at Y:40px */
    padding-bottom: 120px;
  }

  .cta-icon-wrapper {
    width: 160px;
    height: 160px;
    margin-bottom: 120px; /* Text block starts at Y:320. 320 - (40+160) = 120px gap */
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .cta-icon {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .cta-text-content {
    width: 640px;
    max-width: 90vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px; /* Figma gap between title and subtitle */
    margin-bottom: 40px;
  }

  .cta-title {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1.06;
    color: #FAFAFF;
    text-align: center;
    margin: 0;
  }

  .cta-subtitle {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 18px;
    line-height: 1.4;
    color: #FAFAFF;
    opacity: 0.74;
    text-align: center;
    margin: 0;
  }

  .cta-actions {
    display: flex;
    gap: 16px;
    align-items: center;
  }

  .btn-ghost {
    background: transparent;
    border: 1px solid rgba(255, 255, 255, 0.2);
    color: #FAFAFF;
    padding: 12px 24px;
    border-radius: 12px; /* Figma button radius */
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 16px;
    cursor: pointer;
    transition: background 0.2s, border-color 0.2s;
  }

  .btn-ghost:hover {
    background: rgba(255, 255, 255, 0.05);
    border-color: rgba(255, 255, 255, 0.4);
  }

  .btn-primary {
    background: #6A55D7;
    border: none;
    color: #FAFAFF;
    padding: 12px 24px;
    border-radius: 12px;
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 16px;
    cursor: pointer;
    transition: background 0.2s;
  }

  .btn-primary:hover {
    background: #5944b5;
  }

  @media (max-width: 768px) {
    .cta-title {
      font-size: 32px;
    }
    .cta-icon-wrapper {
      margin-bottom: 60px;
    }
    .planet-bg {
      top: 100px;
      width: 120%; 
    }
    .cta-actions {
      flex-direction: row;
      flex-wrap: nowrap;
      gap: 12px;
      width: 100%;
      max-width: 100%;
      justify-content: center;
    }
    .btn-ghost, .btn-primary {
      flex: 1;
      height: 44px;
      padding: 0 12px;
      font-size: 13px;
      white-space: nowrap;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  }
</style>
