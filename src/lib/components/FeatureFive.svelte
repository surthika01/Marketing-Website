<script lang="ts">
  import techImg from '$lib/assets/Group 1437252877.png';
  import unionIcon from '$lib/assets/Union.png';
  import subtractIcon from '$lib/assets/Subtract.png';
  import byobImg from '$lib/assets/Ai - BYOB.png';
  import buildInsideImg from '$lib/assets/AI - Build Inside CometChat.png';
</script>

<section class="feature-five-section">
  <!-- Title Block Layout strictly matching Figma padding and gap -->
  <div class="title-block">
    <div class="tech-image-container">
      <img src={techImg} alt="Technology pathways" class="tech-image" />
    </div>
    
    <div class="text-group">
      <h2 class="main-title">
        Plug In your logic.<br/>
        Or build it here.
      </h2>
      <p class="subtitle">Two paths. Same full-stack experience.</p>
    </div>
  </div>

  <!-- Cards Container Placeholder -->
  <div class="cards-container">
    <!-- Card 1 -->
    <div class="tech-card">
      <div class="card-content">
        <div class="card-icon-container">
          <img src={unionIcon} alt="BYOB Icon" class="card-icon" />
        </div>
        <h3 class="card-title">BYOB - Bring Your Own (Agent) Brain</h3>
        <div class="feature-list">
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Use your existing LLM orchestration</p>
          </div>
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Plug into CometChat's UI, mod, notifications, and insights</p>
          </div>
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Modular, protocol-compatible, and fast to implement</p>
          </div>
        </div>
        <a href="#learn" class="card-link">Learn more</a>
      </div>
      <img src={byobImg} alt="BYOB Architecture" class="card-visual-image" />
    </div>

    <!-- Card 2 -->
    <div class="tech-card">
      <div class="card-content">
        <div class="card-icon-container">
          <img src={subtractIcon} alt="Build Inside CometChat Icon" class="card-icon" />
        </div>
        <h3 class="card-title">Build Inside CometChat</h3>
        <div class="feature-list">
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Visual Agent Builder</p>
          </div>
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Design prompt logic, memory, retries, tool use</p>
          </div>
          <div class="list-item">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
              <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
            </svg>
            <p>Simulate and ship - all from a single canvas</p>
          </div>
        </div>
        <a href="#learn" class="card-link">Learn more</a>
      </div>
      <img src={buildInsideImg} alt="Build Inside Architecture" class="card-visual-image" />
    </div>
  </div>

  <div class="section-divider"></div>
</section>

<style>
  .feature-five-section {
    width: 100%;
    background: #0A0914;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* Figma Title block padding specs */
  .title-block {
    width: 100%;
    max-width: 1440px;
    padding: 100px 64px 48px 64px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px; /* From Figma Gap 10px */
  }

  .tech-image-container {
    width: 100%;
    max-width: 1090px;
    display: flex;
    justify-content: center;
    margin-bottom: 24px;
  }

  .tech-image {
    width: 100%;
    height: auto;
    object-fit: contain;
  }

  .text-group {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px;
  }

  .main-title {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1.06;
    color: #FAFAFF;
    text-align: center;
    margin: 0;
  }

  .subtitle {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 18px; 
    color: #FAFAFF;
    opacity: 0.74;
    text-align: center;
    margin: 0;
  }

  /* Cards basic structure */
  .cards-container {
    width: 100%;
    max-width: 1440px;
    padding: 0 64px 80px 64px;
    display: flex;
    gap: 32px;
    justify-content: center;
  }

  .tech-card {
    flex: 1;
    background: rgba(255, 255, 255, 0.02);
    border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 24px;
    padding: 32px; /* Figma: 576px fill in 640px container = 32px padding */
    display: flex;
    flex-direction: column;
    gap: 32px;
  }

  .card-content {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  .card-icon-container {
    width: 64px;
    height: 64px;
    border: 1px solid rgba(250, 250, 255, 0.1);
    border-radius: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .card-icon {
    width: 32px;
    height: 32px;
    object-fit: contain;
  }

  .card-title {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 640;
    font-size: 24px;
    line-height: 1.06;
    color: #FAFAFF;
    margin: 0;
  }

  .feature-list {
    display: flex;
    flex-direction: column;
    gap: 12px;
  }

  .list-item {
    display: flex;
    align-items: flex-start;
    gap: 12px;
  }

  .list-icon {
    flex-shrink: 0;
    margin-top: 2px;
  }

  .list-item p {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 16px;
    line-height: 1.4;
    color: #FAFAFF;
    opacity: 0.74;
    margin: 0;
  }

  .card-link {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-size: 16px;
    color: #6A55D7;
    text-decoration: none;
    font-weight: 500;
    margin-top: 8px;
  }

  .card-visual-image {
    width: 100%;
    height: auto;
    object-fit: contain;
    margin-top: auto;
  }

  .section-divider {
    width: 1312px;
    max-width: calc(100% - 128px);
    height: 1px;
    background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.2) 20%, rgba(250, 250, 255, 0.2) 80%, rgba(250, 250, 255, 0) 100%);
  }

  @media (max-width: 1024px) {
    .cards-container {
      flex-direction: column;
      padding: 0 20px 64px 20px;
    }
    .title-block {
      padding: 64px 20px 32px 20px;
      align-items: flex-start;
      text-align: left;
    }
    .main-title {
      font-size: 32px;
    }
    .subtitle {
      text-align: left;
    }
  }
</style>
