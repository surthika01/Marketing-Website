<script lang="ts">
  import { base } from '$app/paths';
  let isMenuOpen = $state(false);

  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
</script>

<header class="header">
  <div class="nav-container">
    <a href="{base}/" class="logo">cometchat</a>

    <!-- Desktop Menu (gap: 48px, width: ~500) -->
    <nav class="desktop-nav">
      <a href="#platform">Platform</a>
      <a href="#solutions">Solutions</a>
      <a href="#developers">Developers</a>
      <a href="#resources">Resources</a>
      <a href="#pricing">Pricing</a>
    </nav>

    <div class="nav-right">
      <div class="actions">
        <a href="#login" class="login-link">Log in</a>
        <a href="#demo" class="btn btn-secondary demo-btn">Schedule a demo</a>
      </div>
  
      <!-- Mobile Menu Button -->
      <button
        class="mobile-menu-btn"
        aria-label="Toggle Menu"
        onclick={toggleMenu}
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
        >
          <line x1="3" y1="12" x2="21" y2="12"></line>
          <line x1="3" y1="6" x2="21" y2="6"></line>
          <line x1="3" y1="18" x2="21" y2="18"></line>
        </svg>
      </button>
    </div>
  </div>

  {#if isMenuOpen}
    <nav class="mobile-nav">
      <a href="#platform" onclick={toggleMenu}>Platform</a>
      <a href="#solutions" onclick={toggleMenu}>Solutions</a>
      <a href="#developers" onclick={toggleMenu}>Developers</a>
      <a href="#resources" onclick={toggleMenu}>Resources</a>
      <a href="#pricing" onclick={toggleMenu}>Pricing</a>
      <a href="#login" class="login-link" onclick={toggleMenu}>Log in</a>
      <a href="#demo" class="btn btn-secondary" onclick={toggleMenu}
        >Schedule a demo</a
      >
    </nav>
  {/if}
</header>

<style>
  .header {
    width: 100%;
    background: var(--bg-primary);
    border-bottom: 1px solid #1C1C24;
    position: sticky;
    top: 0;
    z-index: 100;
  }

  .nav-container {
    max-width: 1440px;
    height: 60px;
    margin: 0 auto;
    padding: 12px 16px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    display: flex;
    align-items: center;
    font-family: 'Satoshi Variable', var(--font-sans);
    font-size: 24px;
    font-weight: 700;
    color: #FAFAFF;
    text-decoration: none;
    letter-spacing: -0.02em;
  }

  .desktop-nav {
    display: none;
    align-items: center;
    gap: 48px; /* Exact gap from instructions */
  }

  .desktop-nav a {
    color: #e4e4e7; /* Light gray text for links based on screenshot */
    font-size: 14px;
    font-weight: 500;
    transition: color 0.2s;
  }

  .desktop-nav a:hover {
    color: #fff;
  }

  .nav-right {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .actions {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .demo-btn {
    display: none;
    border-radius: 8px;
  }

  .login-link {
    font-size: 14px;
    font-weight: 500;
    color: #FAFAFF;
  }

  .login-link:hover {
    color: #fff;
  }

  .mobile-menu-btn {
    display: block;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    color: #fff;
    cursor: pointer;
    padding: 6px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background 0.2s;
  }

  .mobile-menu-btn:hover {
    background: rgba(255, 255, 255, 0.1);
  }

  .mobile-nav {
    display: flex;
    flex-direction: column;
    padding: 16px 32px;
    background: var(--bg-secondary);
    gap: 16px;
  }

  .mobile-nav a {
    font-size: 16px;
    color: #fff;
  }

  @media (min-width: 900px) {
    .nav-container {
      height: 68px;
      padding: 16px 32px;
    }
    .desktop-nav {
      display: flex;
    }
    .demo-btn {
      display: inline-flex;
    }
    .mobile-menu-btn {
      display: none;
    }
    .mobile-nav {
      display: none;
    }
  }
</style>
