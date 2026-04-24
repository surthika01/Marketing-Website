<script lang="ts">
  let isMenuOpen = $state(false);

  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
</script>

<header class="header">
  <div class="nav-container">
    <a href="/" class="logo">cometchat</a>

    <!-- Desktop Menu (gap: 48px, width: ~500) -->
    <nav class="desktop-nav">
      <a href="#platform">Platform</a>
      <a href="#solutions">Solutions</a>
      <a href="#developers">Developers</a>
      <a href="#resources">Resources</a>
      <a href="#pricing">Pricing</a>
    </nav>

    <!-- Actions (gap: 16px, width: 197) -->
    <div class="actions">
      <a href="#login" class="login-link">Log in</a>
      <a href="#demo" class="btn btn-primary demo-btn">Schedule a demo</a>
    </div>

    <!-- Mobile Menu Button -->
    <button
      class="mobile-menu-btn"
      aria-label="Toggle Menu"
      on:click={toggleMenu}
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

  {#if isMenuOpen}
    <nav class="mobile-nav">
      <a href="#platform" on:click={toggleMenu}>Platform</a>
      <a href="#solutions" on:click={toggleMenu}>Solutions</a>
      <a href="#developers" on:click={toggleMenu}>Developers</a>
      <a href="#resources" on:click={toggleMenu}>Resources</a>
      <a href="#pricing" on:click={toggleMenu}>Pricing</a>
      <a href="#login" class="login-link" on:click={toggleMenu}>Log in</a>
      <a href="#demo" class="btn btn-primary" on:click={toggleMenu}
        >Schedule a demo</a
      >
    </nav>
  {/if}
</header>

<style>
  .header {
    width: 100%;
    /* border-bottom removed based on screenshot, pure black/dark bg */
    background: var(--bg-primary);
  }

  .nav-container {
    max-width: 1440px;
    height: 68px;
    margin: 0 auto;
    padding: 16px 32px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    display: flex;
    align-items: center;
  }

  .logo img {
    width: 128.8px;
    height: 20px;
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

  .actions {
    display: none;
    align-items: center;
    gap: 16px; /* Exact gap from instructions */
  }

  .login-link {
    font-size: 14px;
    font-weight: 500;
    color: #e4e4e7;
  }

  .login-link:hover {
    color: #fff;
  }

  .demo-btn {
    border-radius: 8px; /* Based on screenshot */
  }

  .mobile-menu-btn {
    display: block;
    background: transparent;
    border: none;
    color: #fff;
    cursor: pointer;
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
    .desktop-nav {
      display: flex;
    }
    .actions {
      display: flex;
    }
    .mobile-menu-btn {
      display: none;
    }
    .mobile-nav {
      display: none;
    }
  }
</style>
