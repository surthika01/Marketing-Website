<script lang="ts">
  import featureImg from '$lib/assets/4b6ce8504aac41e4050fdc65beb0e66b1e337d81.png';
</script>

<section class="feature-three-section">
  <div class="feature-container">
    
    <!-- Left Content (Width: 588px, Gap: 16px) -->
    <div class="feature-content">
      <div class="label">Production-ready chat UI</div>
      
      <h2 class="feature-title">
        The UX layer your agent deserves.<br/>
        Built for LLM-native interactions,<br/>
        out of the box.
      </h2>
      
      <p class="feature-description">
        Forget cobbling together buttons and hoping users 'get it'. Our chat layer is purpose-built for how agents think - and how humans expect them to respond.
      </p>

      <div class="feature-list">
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Token streaming with dynamic "thinking..." states</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Retry/stop buttons with full control logic</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Memory pills, prompt banners, and agent selectors</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Structured tool replies with inline citations</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Slash commands, modals, and frontend triggers</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Low/No-code Chat Builder, or more control via UI Kits and SDKs</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Fully AG-UI protocol compatible - including tool call rendering, memory markers, and fallback patterns</p>
        </div>
      </div>

      <p class="feature-footer">
        It's not just a pretty shell. It's UX that teaches trust, guides behavior, and makes your agent feel alive.
      </p>
    </div>

    <!-- Right Image (Width: 640px, Height: 640px) -->
    <div class="feature-visual">
      <img src={featureImg} alt="Production-ready chat UI" class="feature-img" />
    </div>

  </div>

  <div class="section-divider"></div>
</section>

<style>
  .feature-three-section {
    width: 100%;
    background: #0A0914;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 80px;
    padding-bottom: 0px;
  }

  .section-divider {
    width: 1312px;
    max-width: calc(100% - 128px);
    height: 1px;
    margin-top: 80px;
    background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.2) 20%, rgba(250, 250, 255, 0.2) 80%, rgba(250, 250, 255, 0) 100%);
  }

  /* Inner container matching Figma 1256px wide with 28px gap */
  .feature-container {
    width: 1256px; 
    max-width: 100%;
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    gap: 28px;
    align-items: center;
    padding: 0 32px;
  }

  /* Left content block matching Figma 588px wide with 16px gap */
  .feature-content {
    width: 588px;
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  .label {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 600;
    font-size: 16px;
    color: #6A55D7;
  }

  .feature-title {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 600;
    font-size: 32px;
    line-height: 1.06;
    color: #FAFAFF;
    margin: 0;
  }

  .feature-description {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 18px;
    line-height: 1.2;
    letter-spacing: 0.005em;
    color: #FAFAFF;
    opacity: 0.74;
    margin: 0;
  }

  .feature-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin: 8px 0;
  }

  .list-item {
    display: flex;
    align-items: flex-start;
    gap: 12px;
  }

  .list-icon {
    flex-shrink: 0;
    margin-top: 4px;
  }

  .list-item p {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 18px;
    line-height: 1.2;
    letter-spacing: 0.005em;
    color: #FAFAFF;
    opacity: 0.74;
    margin: 0;
    width: 570px;
    max-width: 100%;
  }

  .feature-footer {
    font-family: 'Satoshi Variable', var(--font-sans);
    font-weight: 500;
    font-size: 18px;
    line-height: 1.2;
    letter-spacing: 0.005em;
    color: #FAFAFF;
    opacity: 0.74;
    margin: 0;
  }

  /* Right visual block matching Figma 640x640px */
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
      gap: 64px;
    }
    
    .feature-content, .feature-visual {
      width: 100%;
    }
    
    .feature-visual {
      height: auto;
      aspect-ratio: 1/1;
    }
  }
</style>
