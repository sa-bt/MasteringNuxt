<template>
  <div>
    <Html :lang="dynamic > 50 ? 'en-GB' : 'en-US'">
      <Head>
        <Title>Top 50 Restaurant in the World</Title>
        <Meta name="description" content="My page is cool"></Meta>
        <Link
          rel="preload"
          href="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
          as="script"
        /> </Head
    >
  </Html>

    <NuxtLayout name="custom">
      <div class="container">
        <RestaurantTable />
      </div>
    </NuxtLayout>
  </div>
</template>
<style scoped>
.container {
  text-align: center;
  margin-top: 5rem;
}
</style>
