<footer class="footer">
  <div class="watermark">cometchat</div>
  
  <div class="container">
    <div class="footer-top">
      <div class="logo-container">
        <span class="logo">cometchat</span>
      </div>
    </div>

    <div class="footer-grid">
      <!-- Column 1: Platform -->
      <div class="link-col">
        <h4>Platform</h4>
        <nav>
          <a href="#chat">Chat & Messaging</a>
          <a href="#voice">Voice & Video Calls</a>
          
          <span class="sub-header">Features</span>
          <a href="#chat-messaging">Chat & Messaging</a>
          <a href="#voice-calls">Voice & Video Calls</a>
          <a href="#notifications">Notifications</a>
          <a href="#analytics">Analytics & Insights</a>
          <a href="#multi-tenant">Multi-Tenant Chat</a>
          
          <span class="sub-header">Integration Methods</span>
          <a href="#ui-kits">UI Kits</a>
          <a href="#sdks">SDKs & APIs</a>
        </nav>
      </div>

      <!-- Column 2: Solutions -->
      <div class="link-col">
        <h4>Solutions</h4>
        <nav>
          <span class="sub-header">By Use cases</span>
          <a href="#on-demand">On-demand</a>
          <a href="#marketplaces">Online Marketplaces</a>
          <a href="#saas">SaaS Businesses</a>
          <a href="#healthcare">Healthcare & Telehealth</a>
          <a href="#community">Community & Social</a>
          <a href="#dating">Dating</a>
          
          <span class="sub-header">Comparison</span>
          <a href="#vs-sendbird">CometChat vs Sendbird</a>
          <a href="#compare-top">Compare Top Chat SDKs</a>
          <a href="#sendbird-alt">Sendbird Alternatives</a>
          <a href="#stream-alt">Stream Chat Alternatives</a>
        </nav>
      </div>

      <!-- Column 3: Developers -->
      <div class="link-col">
        <h4>Developers</h4>
        <nav>
          <a href="#docs">Docs</a>
          <a href="#sample-apps">Sample Apps</a>
          <a href="#apis">APIs</a>
          <a href="#updates">Product Updates</a>
          <a href="#requests">Feature Requests</a>
          <a href="#status">System Status</a>
          
          <span class="sub-header">Support</span>
          <a href="#community">Community</a>
          <a href="#help">Help Center</a>
          <a href="#office-hours">Office Hours</a>
          <a href="#report">Report an issue</a>
        </nav>
      </div>

      <!-- Column 4: Resources -->
      <div class="link-col">
        <h4>Resources</h4>
        <nav>
          <a href="#templates">Templates</a>
          <a href="#tutorials">Tutorials</a>
          <a href="#blog">Blog</a>
          
          <span class="sub-header">Chat UI Kits</span>
          <a href="#react">React Chat UI Kit</a>
          <a href="#flutter">Flutter Chat UI Kit</a>
          <a href="#android">Android Chat UI Kit</a>
          <a href="#react-native">React Native Chat UI Kit</a>
          <a href="#ios">iOS Chat UI Kit</a>
        </nav>
      </div>

      <!-- Column 5: Company -->
      <div class="link-col">
        <h4>Company</h4>
        <nav>
          <a href="#careers">Careers</a>
          <a href="#partners">Partners</a>
          <a href="#pricing">Pricing</a>
          <a href="#implementation">Implementation Services</a>
          <a href="#chat-with-us">Chat with us</a>
          
          <span class="sub-header">Terms and Legal</span>
          <a href="#tos">Terms of Service</a>
          <a href="#privacy">Privacy Policy</a>
          <a href="#subprocessors">Sub-processors List</a>
          <a href="#dpa">Data Processing Addendum</a>
          <a href="#vulnerability">Vulnerability Disclosure Program</a>
        </nav>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="legal">
        <span>2025 © CometChat</span>
        <a href="#tos">Terms of Use</a>
        <a href="#privacy">Privacy Policy</a>
      </div>
      <div class="socials">
        <a href="#linkedin" class="social-link">LinkedIn</a>
        <a href="#instagram" class="social-link">Instagram</a>
        <a href="#twitter" class="social-link">Twitter</a>
        <a href="#github" class="social-link">GitHub</a>
      </div>
    </div>
  </div>
</footer>

<style>
  .footer {
    width: 100%;
    background-color: #0A0914;
    padding-top: 56px;
    padding-bottom: 40px;
    position: relative;
    overflow: hidden;
    margin-top: auto;
    font-family: 'Satoshi Variable', var(--font-sans);
  }

  .watermark {
    position: absolute;
    bottom: -40px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 200px;
    font-weight: 800;
    color: rgba(255, 255, 255, 0.015);
    pointer-events: none;
    line-height: 1;
    z-index: 0;
    white-space: nowrap;
    user-select: none;
  }

  .container {
    max-width: 1440px;
    margin: 0 auto;
    padding: 0 64px;
    position: relative;
    z-index: 1;
  }

  .footer-top {
    margin-bottom: 48px;
  }

  .logo {
    font-size: 24px;
    font-weight: 700;
    color: #FAFAFF;
    letter-spacing: -0.02em;
  }

  .footer-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 40px;
    margin-bottom: 80px;
  }

  .link-col {
    display: flex;
    flex-direction: column;
  }

  .link-col h4 {
    font-size: 16px;
    font-weight: 600;
    color: #6852D6;
    margin: 0 0 24px 0;
  }

  nav {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  nav a {
    color: #FAFAFF;
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    opacity: 0.74;
    transition: opacity 0.2s, color 0.2s;
  }

  nav a:hover {
    opacity: 1;
    color: #6852D6;
  }

  .sub-header {
    color: #FAFAFF;
    font-size: 14px;
    font-weight: 600;
    opacity: 0.9;
    margin-top: 16px;
    display: block;
  }

  .footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 1px solid rgba(255, 255, 255, 0.05);
    padding-top: 32px;
  }

  .legal {
    display: flex;
    align-items: center;
    gap: 24px;
  }

  .legal span, .legal a {
    color: #FAFAFF;
    opacity: 0.6;
    font-size: 14px;
    text-decoration: none;
    font-weight: 500;
  }

  .socials {
    display: flex;
    gap: 24px;
  }

  .social-link {
    color: #FAFAFF;
    opacity: 0.6;
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    transition: opacity 0.2s;
  }

  .social-link:hover {
    opacity: 1;
  }

  @media (max-width: 1024px) {
    .footer-grid {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media (max-width: 640px) {
    .footer-grid {
      grid-template-columns: 1fr;
    }
  }
</style>
