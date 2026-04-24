<script lang="ts">
  import footerContent from '$lib/assets/Content.png';
</script>

<footer class="footer">
  <div class="container">
    <img src={footerContent} alt="CometChat Footer Content" class="footer-img" />
  </div>
</footer>

<style>
  .footer {
    width: 100%;
    background-color: #0A0914;
    padding-top: 56px;
    padding-bottom: 40px;
    display: flex;
    justify-content: center;
  }

  .container {
    width: 100%;
    max-width: 1440px;
    padding: 0 64px;
  }

  .footer-img {
    width: 100%;
    height: auto;
    object-fit: contain;
    display: block;
  }

  @media (max-width: 768px) {
    .container {
      padding: 0 20px;
    }
  }
</style>
