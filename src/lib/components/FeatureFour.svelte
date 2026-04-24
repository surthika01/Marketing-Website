<script lang="ts">
  import featureImg from '$lib/assets/714ad9a443db19b0f911d336ab5796d2124d967d.png';
</script>

<section class="feature-four-section">
  <div class="feature-container">
    
    <!-- Left Content (Width: 588px, Gap: 16px) -->
    <div class="feature-content">
      <div class="label">Multichannel notifications engine</div>
      
      <h2 class="feature-title">
        Your agent is only helpful if people<br class="desktop-br" />
        come back to talk to it.
      </h2>
      
      <p class="feature-description">
        Most agents get ghosted. Yours won't.
      </p>

      <div class="feature-list">
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Native push, email, and SMS support</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Retry logic, delivery throttling, and batching</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Trigger-based delivery rules - unread X mins, fallback triggered, user went silent</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Threaded email replies (yes, replies go back to chat!)</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>Integrates with SendGrid, Twilio, or your custom providers</p>
        </div>
        <div class="list-item">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" class="list-icon">
            <path d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z" fill="#6A55D7"/>
          </svg>
          <p>User-level frequency + preference settings</p>
        </div>
      </div>

      <p class="feature-footer">
        Notifications aren't a growth hack. They're UX glue. And we built them so you wouldn't have to.
      </p>
    </div>

    <!-- Right Image (Width: 640px, Height: 640px) -->
    <div class="feature-visual">
      <img src={featureImg} class="feature-img" alt="Multichannel notifications engine" />
    </div>

  </div>

  <div class="section-divider"></div>
</section>

<style>
  .feature-four-section {
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
    text-align: left;
  }

  .desktop-br {
    display: block;
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
      align-items: flex-start;
      gap: 64px;
    }
    
    .feature-content, .feature-visual {
      width: 100%;
      align-items: flex-start;
      text-align: left;
    }

    .desktop-br {
      display: none;
    }
    
    .feature-visual {
      height: auto;
      aspect-ratio: 1/1;
      align-self: center;
    }
  }
</style>
