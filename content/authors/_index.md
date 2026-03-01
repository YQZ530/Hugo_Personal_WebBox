---
# To publish author profile pages, remove all the `build` and `cascade` settings below.
build:
  render: never
cascade:
  build:
    render: never
    list: always

website_url: "https://yqz530.github.io/"
---
<style>
  /* Optional: This hides the author box entirely if you'd rather have no bio section */
  /* .flex.pt-12.pb-4 { display: none !important; } */
</style>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    // Finds the link to your name in the author bio section at the bottom
    const bioLinks = document.querySelectorAll('a[href*="/authors/"], a[href*="localhost:1313"]');
    
    bioLinks.forEach(link => {
      // Check if it's the link to your profile
      if (link.textContent.trim().includes('Yongqi Zhang')) {
        link.href = 'https://yqz530.github.io/';
      }
    });
  });
</script>