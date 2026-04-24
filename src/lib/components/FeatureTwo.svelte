<script lang="ts">
  import featureImg from "$lib/assets/Image.png";
</script>

<section class="feature-two-section">
  <div class="feature-container">
    <!-- Left Content -->
    <div class="feature-content">
      <h2 class="feature-title">
        Everything you'd end up<br />
        <span class="text-gradient">already done.</span>
      </h2>

      <div class="feature-list">
        <div class="list-item">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            class="list-icon"
          >
            <path
              d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z"
              fill="#6A55D7"
            />
          </svg>
          <p>
            A complete frontend and system layer for AI agents. Plug in your LLM
            backend or build the brain with ours.
          </p>
        </div>
        <div class="list-item">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            class="list-icon"
          >
            <path
              d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z"
              fill="#6A55D7"
            />
          </svg>
          <p>
            CometChat is the only full stack agent platform that combines logic,
            UI, moderation, notifications, and insights - without glue code.
          </p>
        </div>
        <div class="list-item">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            class="list-icon"
          >
            <path
              d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z"
              fill="#6A55D7"
            />
          </svg>
          <p>
            Each of these is battle-tested, used and trusted in production by
            real companies, across real user scenarios.
          </p>
        </div>
      </div>
    </div>

    <!-- Right Image -->
    <div class="feature-visual">
      <img
        src={featureImg}
        alt="Feature visual already done"
        class="feature-img"
      />
    </div>
  </div>

  <div class="section-divider"></div>
</section>

<style>
  .feature-two-section {
    width: 100%;
    background: #0a0914;
    display: flex;
    flex-direction: column;
    align-items: center;
    /* padding-top: 80px; */
    padding-bottom: 0px; /* Padding below line will be handled by next section or added here */
  }

  .section-divider {
    width: 1312px;
    max-width: calc(100% - 128px);
    height: 1px;
    margin-top: 80px;
    background: linear-gradient(
      90deg,
      rgba(250, 250, 255, 0) 0%,
      rgba(250, 250, 255, 0.2) 20%,
      rgba(250, 250, 255, 0.2) 80%,
      rgba(250, 250, 255, 0) 100%
    );
  }

  .feature-container {
    width: 1440px;
    max-width: 100%;
    padding: 0 64px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .feature-content {
    width: max-content; /* Allow children to dictate width */
    max-width: 100%;
    display: flex;
    flex-direction: column;
    gap: 40px;
  }

  .feature-title {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1.06;
    letter-spacing: 0;
    color: #fafaff;
    margin: 0;
  }

  .text-gradient {
    background: var(--gradient-text);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    color: transparent;
  }

  .feature-list {
    display: flex;
    flex-direction: column;
    gap: 16px; /* Based on Gap: 16px in Image 4 */
  }

  .list-item {
    display: flex;
    align-items: flex-start;
    gap: 16px;
  }

  .list-icon {
    flex-shrink: 0;
    width: 20px;
    height: 20px;
    margin-top: 4px; /* align with the 22px text */
  }

  .list-item p {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 500;
    font-size: 22px;
    line-height: 1.2;
    letter-spacing: 0.005em;
    color: #fafaff;
    opacity: 0.74;
    margin: 0;
    width: 570px;
    max-width: 100%;
  }

  .feature-visual {
    width: 640px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .feature-img {
    width: 100%;
    height: auto;
    object-fit: contain;
  }

  @media (max-width: 1200px) {
    .feature-container {
      flex-direction: column;
      align-items: flex-start;
      height: auto;
      gap: 64px;
      padding: 60px 32px;
    }

    .feature-content {
      width: 100%;
    }

    .feature-title {
      font-size: 32px;
    }

    .list-item p {
      font-size: 16px;
      width: 100%;
    }

    .feature-visual {
      width: 100%;
      height: auto;
    }
  }
</style>
