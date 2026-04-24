<script lang="ts">
  import icon1 from "$lib/assets/Union.png";
  import icon2 from "$lib/assets/star-06.png";
  import icon3 from "$lib/assets/Subtract.png";

  const cards = [
    {
      title: "Chat Builder",
      desc: "The fastest way to go live.",
      icon: icon1,
      bullets: [
        "Visual interface for styling and configuring chat",
        "Drop into any web or mobile app with a single snippet",
        "Integrates with auth, analytics, and third-party tools",
        "Great for prototypes, pilots, or teams with limited frontend resources",
      ],
    },
    {
      title: "UI Kits",
      desc: "Production-ready components with full flexibility.",
      icon: icon2,
      bullets: [
        "Available for all popular frameworks",
        "Theming, layout, and logic hooks exposed",
        "Save time on structure, focus on experience",
        "Ideal for teams who want speed and polish",
      ],
    },
    {
      title: "SDKs & APIs",
      desc: "The toolbox for when you want total control.",
      icon: icon3,
      bullets: [
        "Available for all popular frameworks",
        "Theming, layout, and logic hooks exposed",
        "Save time on structure, focus on experience",
        "Ideal for teams who want speed and polish",
      ],
    },
  ];
</script>

<section class="feature-six-section">
  <!-- Title Block Layout matching Figma specs -->
  <div class="title-block">
    <div class="text-group">
      <span class="pre-title">Chat integration options</span>
      <h2 class="main-title">Your launch, your way. Done right.</h2>
      <p class="subtitle">
        Start with what gets you to production fastest — or matches your needs
        the best.<br />
        Swap it out or level it up later.
      </p>
    </div>
  </div>

  <div class="cards-wrapper">
    <div class="cards-bg-line">
      <div class="node left-node"></div>
      <div class="node right-node"></div>
    </div>

    <div class="cards-container">
      {#each cards as card}
        <div class="integration-card">
          <div class="card-icon-container">
            <img src={card.icon} alt="{card.title} Icon" class="card-icon" />
          </div>

          <div class="card-content-inner">
            <h3 class="card-title">{card.title}</h3>

            <p class="card-desc">{card.desc}</p>

            <div class="hover-content">
              {#each card.bullets as bullet}
                <div class="list-item">
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 24 24"
                    fill="none"
                    class="list-icon"
                  >
                    <path
                      d="M12 2L14.5 9.5L22 12L14.5 14.5L12 22L9.5 14.5L2 12L9.5 9.5L12 2Z"
                      fill="#6A55D7"
                    />
                  </svg>
                  <p>{bullet}</p>
                </div>
              {/each}
            </div>

            <a href="#try" class="card-link">Try Builder</a>
          </div>
        </div>
      {/each}
    </div>
  </div>

  <div class="section-divider"></div>
</section>

<style>
  .feature-six-section {
    width: 100%;
    background: #0a0914;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* Title Block */
  .title-block {
    width: 100%;
    max-width: 1440px;
    padding: 100px 64px 48px 64px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .text-group {
    width: 100%;
    max-width: 858px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 12px;
  }

  .pre-title {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 600;
    font-size: 22px;
    line-height: 1.06;
    color: #6852d6;
    text-align: center;
    margin: 0;
  }

  .main-title {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 600;
    font-size: 48px;
    line-height: 1.06;
    color: #fafaff;
    text-align: center;
    margin: 0;
  }

  .subtitle {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 500;
    font-size: 18px;
    color: #fafaff;
    opacity: 0.74;
    text-align: center;
    line-height: 1.4;
    margin: 0;
    margin-top: 8px;
  }

  /* Cards Setup */
  .cards-wrapper {
    width: 100%;
    max-width: 1440px;
    /* padding: 48px 64px 80px 64px; */
    position: relative;
  }

  .cards-bg-line {
    position: absolute;
    top: 48px; /* Matches padding top */
    left: 64px;
    right: 64px;
    height: 1px;
    background: rgba(255, 255, 255, 0.05);
    z-index: 1;
  }

  .node {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    border: 1px solid rgba(255, 255, 255, 0.1);
    background: #0a0914;
    position: absolute;
    top: -5px; /* Center node on line */
  }

  .left-node {
    left: -6px;
  }
  .right-node {
    right: -6px;
  }

  .cards-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    position: relative;
    z-index: 2;
  }

  .integration-card {
    display: flex;
    flex-direction: column;
    padding: 40px 32px 32px 32px;
    position: relative;
    border: 1px solid transparent; /* Prepare for hover */
    transition: all 0.3s ease;
    border-radius: 12px;
  }

  .integration-card:not(:last-child) {
    border-right: 1px solid rgba(255, 255, 255, 0.05);
  }

  /* Icon Setup */
  .card-icon-container {
    width: 64px;
    height: 64px;
    background: #0a0914;
    border: 1px solid rgba(250, 250, 255, 0.1);
    border-radius: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    top: -32px;
    left: 40px;
    transition:
      opacity 0.2s ease,
      transform 0.2s ease;
  }

  .card-icon {
    width: 32px;
    height: 32px;
    object-fit: contain;
  }

  /* Text & Content */
  .card-content-inner {
    margin-top: 24px;
    display: flex;
    flex-direction: column;
    transition: margin-top 0.3s ease;
  }

  .card-title {
    font-family: "Satoshi Variable", var(--font-sans);
    font-weight: 600;
    font-size: 24px;
    color: #fafaff;
    margin: 0;
    margin-bottom: 8px;
  }

  .card-desc {
    font-family: "Satoshi Variable", var(--font-sans);
    font-size: 16px;
    color: #fafaff;
    opacity: 0.74;
    margin: 0;
    line-height: 1.4;
    transition: opacity 0.2s ease;
  }

  .hover-content {
    display: none;
    flex-direction: column;
    gap: 12px;
    opacity: 0;
    margin-top: 8px;
    margin-bottom: 16px;
    transition: opacity 0.3s ease;
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
    font-family: "Satoshi Variable", var(--font-sans);
    font-size: 14px;
    color: #fafaff;
    opacity: 0.8;
    margin: 0;
    line-height: 1.4;
  }

  .card-link {
    font-family: "Satoshi Variable", var(--font-sans);
    font-size: 16px;
    color: #6a55d7;
    text-decoration: none;
    font-weight: 500;
    margin-top: auto; /* Push down */
    padding-top: 16px;
  }

  /* HOVER ANIMATION STATES */
  .integration-card:hover {
    background: radial-gradient(
      120% 120% at 0% 0%,
      rgba(104, 82, 214, 0.15) 0%,
      rgba(104, 82, 214, 0) 100%
    );
    border: 1px solid rgba(104, 82, 214, 0.6);
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
    border-right: 1px solid rgba(104, 82, 214, 0.6) !important;
    z-index: 10;
  }

  .integration-card:hover .card-icon-container {
    opacity: 0;
    transform: translateY(-10px);
    pointer-events: none;
  }

  .integration-card:hover .card-content-inner {
    margin-top: 0; /* Move content up to fill space left by icon */
  }

  .integration-card:hover .card-desc {
    display: none; /* Hide short desc immediately */
  }

  .integration-card:hover .hover-content {
    display: flex;
    opacity: 1;
    animation: fadeIn 0.3s ease forwards;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(5px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  /* Base Separator line below block */
  .section-divider {
    width: 1312px;
    max-width: calc(100% - 128px);
    height: 1px;
    background: linear-gradient(
      90deg,
      rgba(250, 250, 255, 0) 0%,
      rgba(250, 250, 255, 0.2) 20%,
      rgba(250, 250, 255, 0.2) 80%,
      rgba(250, 250, 255, 0) 100%
    );
  }

  @media (max-width: 1024px) {
    .title-block {
      padding: 64px 20px 32px 20px;
      align-items: center;
      text-align: center;
    }

    .main-title {
      font-size: 32px;
    }

    .pre-title {
      font-size: 18px;
    }

    .cards-container {
      grid-template-columns: 1fr;
      gap: 32px;
    }

    .integration-card {
      padding: 40px 24px 24px 24px;
      border: 1px solid rgba(255, 255, 255, 0.05);
      background: rgba(255, 255, 255, 0.02);
      border-right: 1px solid rgba(255, 255, 255, 0.05) !important;
    }

    .card-icon-container {
      position: relative;
      top: 0;
      left: 0;
      margin-bottom: 24px;
      opacity: 1 !important;
      transform: none !important;
    }

    .card-content-inner {
      margin-top: 0;
    }

    .card-desc {
      display: block !important;
      opacity: 1;
      margin-bottom: 16px;
    }

    .hover-content {
      display: flex;
      opacity: 1;
      margin-top: 16px;
    }

    /* Disable desktop hover effects on mobile */
    .integration-card:hover {
      background: rgba(255, 255, 255, 0.02);
      border: 1px solid rgba(255, 255, 255, 0.05);
      transform: none;
    }

    .integration-card:hover .card-icon-container {
      opacity: 1;
      transform: none;
    }

    .integration-card:hover .card-desc {
      display: block;
    }

    .cards-bg-line {
      display: none;
    }
  }
</style>
