<script lang="ts">
  import { base } from '$app/paths';
  import footerLogo from '$lib/assets/CometChat Logo.png';
</script>

<footer class="footer">
  <div class="container">
    <div class="footer-top">
      <div class="logo-container">
        <a href="{base}/" class="logo">cometchat</a>
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

    <div class="footer-visual">
      <img src={footerLogo} alt="CometChat" class="large-outline-logo" />
    </div>

    <div class="footer-bottom">
      <div class="legal">
        <span>2025 © CometChat</span>
        <a href="#tos">Terms of Use</a>
        <a href="#privacy">Privacy Policy</a>
      </div>
      <div class="socials">
        <a href="#linkedin" class="social-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
          LinkedIn
        </a>
        <a href="#instagram" class="social-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg>
          Instagram
        </a>
        <a href="#twitter" class="social-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"/></svg>
          Twitter
        </a>
        <a href="#github" class="social-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
          GitHub
        </a>
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
    margin-top: auto;
    font-family: 'Satoshi Variable', var(--font-sans);
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
    display: flex;
    justify-content: space-between;
    gap: 24px;
    margin-bottom: 80px;
    flex-wrap: wrap;
  }

  .link-col {
    display: flex;
    flex-direction: column;
    min-width: 180px;
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

  .footer-visual {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-bottom: 64px;
    pointer-events: none;
  }

  .large-outline-logo {
    width: 100%;
    max-width: 1313px;
    height: auto;
    opacity: 1; /* Fully visible for debugging */
    object-fit: contain;
    border: 2px solid #191822;
    border-radius: 12px;
    padding: 20px;
    display: block;
  }

  .footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 1px dashed rgba(255, 255, 255, 0.1);
    padding-top: 32px;
    flex-wrap: wrap;
    gap: 24px;
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

  .legal a:hover {
    opacity: 1;
  }

  .socials {
    display: flex;
    gap: 24px;
    align-items: center;
  }

  .social-link {
    display: flex;
    align-items: center;
    gap: 8px;
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
    .container {
      padding: 0 32px;
    }
    .footer-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 48px;
    }
  }

  @media (max-width: 640px) {
    .footer-grid {
      grid-template-columns: 1fr;
    }
    .footer-bottom {
      flex-direction: column;
      align-items: flex-start;
    }
  }
</style>
