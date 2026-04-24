<script lang="ts">
  import Header from '$lib/components/Header.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Feature from '$lib/components/Feature.svelte';
  import FeatureTwo from '$lib/components/FeatureTwo.svelte';
  import FeatureThree from '$lib/components/FeatureThree.svelte';
  import FeatureFour from '$lib/components/FeatureFour.svelte';
  import FeatureFive from '$lib/components/FeatureFive.svelte';
  import FeatureSix from '$lib/components/FeatureSix.svelte';
  import CTA from '$lib/components/CTA.svelte';
  import Footer from '$lib/components/Footer.svelte';

  const seoTitle = "CometChat - Build In-App Chat Faster";
  const seoDescription = "The complete chat infrastructure that scales with your application. Add secure, reliable messaging to your product in minutes.";
  const canonicalUrl = "https://www.cometchat.com/";
  
  // JSON-LD Structured Data
  const jsonLd = {
    "@context": "https://schema.org",
    "@type": "SoftwareApplication",
    "name": "CometChat",
    "operatingSystem": "All",
    "applicationCategory": "DeveloperApplication",
    "description": seoDescription,
    "url": canonicalUrl,
    "publisher": {
      "@type": "Organization",
      "name": "CometChat"
    }
  };
</script>

<svelte:head>
  <!-- Technical SEO Requirements -->
  <title>{seoTitle}</title>
  <meta name="description" content={seoDescription} />
  <link rel="canonical" href={canonicalUrl} />
  
  <!-- Open Graph Basic -->
  <meta property="og:title" content={seoTitle} />
  <meta property="og:description" content={seoDescription} />
  <meta property="og:type" content="website" />
  <meta property="og:url" content={canonicalUrl} />
  
  <script type="application/ld+json">
    {@html JSON.stringify(jsonLd)}
  </script>
</svelte:head>

<Header />

<main>
  <Hero />
  <Feature />
  <FeatureTwo />
  <FeatureThree />
  <FeatureFour />
  <FeatureFive />
  <FeatureSix />
  <CTA />
</main>

<Footer />

<style>
  main {
    flex: 1;
    display: flex;
    flex-direction: column;
  }
</style>
