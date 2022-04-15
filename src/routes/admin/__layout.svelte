<slot />

<style lang="scss">
  @import url("https://fonts.googleapis.com/css2?family=Inter:wght@500&family=Manrope:wght@200;300;400;500;600;700;800&display=swap");

  :root {
    font-family: "Manrope", sans-serif;
  }

  :global(html) {
    box-sizing: border-box;
    font-size: 16px;
  }
  :global(body, h1, h2, h3, h4, h5, h6, p, ol, ul, input, button) {
    margin: 0;
    padding: 0;
    font-family: inherit;
  }
  :global(ol, ul) {
    list-style: none;
  }
  :global(img) {
    max-width: 100%;
    height: auto;
  }
</style>
