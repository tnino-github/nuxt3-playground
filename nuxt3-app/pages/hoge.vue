<script setup lang="ts">
  const { data: title } = await useFetch("/api/hello");
</script>

<template>
  <Html lang="ja">
    <Head>
      <Title>Hoge</Title>
      <Meta name="description" :content="`This is sample page`" />
    </Head>
  </Html>

  <h1>{{ title }}</h1>
</template>
