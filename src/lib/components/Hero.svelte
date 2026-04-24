<script lang="ts">
  import bannerImg from '$lib/assets/Banner images.png';
</script>

<section class="hero-section">
  <div class="hero-container">
    
    <!-- Left Layout (Width: 528px, Gap: 32px) -->
    <div class="hero-content">
      
      <!-- Pill -->
      <div class="pill">
        <div class="pill-icon">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            <path d="M5.5 4.5L6.5 7L9 8L6.5 9L5.5 11.5L4.5 9L2 8L4.5 7L5.5 4.5Z" fill="#6A55D7"/>
          </svg>
        </div>
        <span class="pill-text">Full Stack AI Agent Platform</span>
      </div>
      
      <h1 class="hero-title">
        Ship the <span class="text-gradient">agent.</span><br/>
        Skip the <span class="text-gradient">plumbing.</span>
      </h1>
      
      <p class="hero-description">
        Why are you still stitching together chat UIs, retries, moderation, notifications, and analytics - just to get your agent into users' hands?<br/><br/>
        CometChat gives you the entire frontend + infra layer. Full stack. Modular. Production-ready.
      </p>
      
      <div class="hero-actions">
        <a href="#demo" class="btn btn-secondary">Schedule a Demo</a>
        <a href="#builder" class="btn btn-primary">Try the Agent Builder</a>
      </div>
    </div>
    
    <!-- Right Layout (Width: 575.75px, Height: 475px) -->
    <div class="hero-visual">
      <!-- We will place the exported asset here as requested "Banner images us ethst image beloow" -->
      <!-- Since asset is not physically present in filesystem, we use a structured placeholder matching the layout -->
      <div class="banner-image-placeholder">
        <img src={bannerImg} alt="AI Agent Platform Interface" class="banner-img" />
      </div>
    </div>

  </div>
  
  <!-- Trusted By Section -->
  <div class="trusted-by-section">
    <!-- Rectangle 844 (Glass container) -->
    <div class="trusted-rectangle">
      <!-- Scrolling track inside -->
      <div class="trusted-track">
        <div class="logo-group">
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/43/Haleon_logo.svg" alt="Haleon" class="trusted-logo" />
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Kahoot_Logo.svg" alt="Kahoot" class="trusted-logo" />
          <span class="trusted-text-logo">shaadi.com</span>
          <span class="trusted-text-logo">endeavor</span>
          <span class="trusted-text-logo">NOBROKER</span>
        </div>
        <div class="logo-group" aria-hidden="true">
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/43/Haleon_logo.svg" alt="Haleon" class="trusted-logo" />
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Kahoot_Logo.svg" alt="Kahoot" class="trusted-logo" />
          <span class="trusted-text-logo">shaadi.com</span>
          <span class="trusted-text-logo">endeavor</span>
          <span class="trusted-text-logo">NOBROKER</span>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .hero-section {
    padding-top: 100px;
    display: flex;
    flex-direction: column;
    align-items: center;
    background: var(--bg-primary);
  }

  .hero-container {
    max-width: 1440px;
    width: 100%;
    margin: 0 auto;
    padding: 0 32px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
  }

  /* Left Content Layout */
  .hero-content {
    width: 528px;
    display: flex;
    flex-direction: column;
    gap: 32px; /* Exact gap specified */
  }

  .pill {
    width: max-content;
    height: 44px;
    padding: 6px 20px 6px 6px;
    border-radius: 99px;
    border: 1px solid transparent;
    /* Use solid #0A0914 inside to avoid the gray overlay, then gradient for border */
    background-image: linear-gradient(#0A0914, #0A0914), 
                      linear-gradient(180deg, #FFFFFF 0%, #6A55D7 126.95%);
    background-origin: border-box;
    background-clip: padding-box, border-box;
    display: flex;
    align-items: center;
    gap: 12px;
  }
  
  .pill-icon {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: linear-gradient(135deg, #FFFFFF 0%, #F0D0FF 100%);
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .pill-text {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-size: 18px;
    font-weight: 600;
    line-height: 1.12;
    letter-spacing: 0;
    text-align: center;
    color: #C2B0FF; /* Solid light purple matching Image 1 */
    white-space: nowrap;
  }

  .hero-title {
    font-size: 56px;
    line-height: 1.1;
    font-weight: 500;
    letter-spacing: -0.02em;
    color: #FFFFFF;
  }

  .hero-description {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-size: 22px;
    font-weight: 500;
    line-height: 1.2;
    letter-spacing: 0.005em;
    color: #FAFAFF;
    max-width: 528px;
  }

  .hero-actions {
    display: flex;
    gap: 12px;
    height: 44px;
  }

  .hero-actions .btn {
    padding: 0 24px;
    font-size: 15px;
    border-radius: 8px;
    height: 100%;
  }

  /* Right Visual Layout */
  .hero-visual {
    width: 575.75px;
    height: 475px;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .banner-image-placeholder {
    width: 100%;
    height: 100%;
    position: relative;
    border-radius: 16px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .banner-img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: contain;
    z-index: 2;
  }



  /* Trusted By Section (Parent Container) */
  .trusted-by-section {
    width: 100%;
    max-width: 1312px;
    height: 136px;
    margin: 60px auto 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }
  
  /* Rectangle 844 (Glass container) */
  .trusted-rectangle {
    width: 1047px;
    height: 86px;
    background: rgba(10, 9, 20, 0.5); /* #0A0914 50% */
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border: 1px solid rgba(255, 255, 255, 0.05); /* Slight border to define the glass shape */
    position: relative;
    overflow: hidden; /* Hide the scrolling elements outside container */
    display: flex;
    align-items: center;
  }

  /* Fade edges inside the rectangle for smooth scroll entry/exit */
  .trusted-rectangle::before,
  .trusted-rectangle::after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    width: 100px;
    z-index: 2;
  }
  
  .trusted-rectangle::before {
    left: 0;
    background: linear-gradient(to right, rgba(10, 9, 20, 0.8) 0%, transparent 100%);
  }
  
  .trusted-rectangle::after {
    right: 0;
    background: linear-gradient(to left, rgba(10, 9, 20, 0.8) 0%, transparent 100%);
  }

  .trusted-track {
    display: flex;
    width: max-content;
    opacity: 0.6;
    animation: scroll-marquee 30s linear infinite;
  }

  .trusted-track:hover {
    animation-play-state: paused;
  }

  .logo-group {
    display: flex;
    align-items: center;
    gap: 80px;
    padding-right: 80px;
  }

  @keyframes scroll-marquee {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }

  .trusted-logo {
    height: 30px;
    filter: grayscale(100%) brightness(200%);
  }
  
  .trusted-text-logo {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-size: 14px;
    font-weight: 600;
    line-height: 1.4;
    letter-spacing: 0.02em;
    color: #FAFAFF;
  }

  @media (max-width: 1100px) {
    .hero-container {
      flex-direction: column;
      text-align: left;
      align-items: flex-start;
      gap: 32px;
    }
    
    .hero-content {
      align-items: flex-start;
      width: 100%;
    }

    .hero-title {
      font-size: 32px; /* Smaller title for mobile */
      line-height: 1.1;
    }
    
    .hero-description {
      text-align: left;
      font-size: 16px; /* Smaller font for mobile */
    }

    .hero-actions {
      flex-direction: row;
      flex-wrap: wrap;
      height: auto;
      gap: 12px;
    }

    .hero-visual {
      width: 100%;
      height: auto;
      aspect-ratio: 1.2;
    }
    
    .logo-group {
      gap: 40px;
      padding-right: 40px;
    }
  }
</style>
