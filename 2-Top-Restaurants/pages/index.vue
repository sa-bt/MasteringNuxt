<template>
  <div>
    <Html :lang="dynamic > 50 ? 'en-GB' : 'en-US'">
      <Head>
        <Title>Restaurantly</Title>
        <Meta name="description" content="My page is cool"></Meta>
        <Link
          rel="preload"
          href="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
          as="script"
        /> </Head
    ></Html>
    <div class="container">
      <h1>Welcome to Restaurantly</h1>
      <a href="/restaurants">Go to restaurants</a>
    </div>
  </div>
</template>
<style scoped>
.container {
  text-align: center;
  margin-top: 5rem;
}
</style>
