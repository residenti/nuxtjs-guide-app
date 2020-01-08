<template>
  <div>
    <h2>users/_id/index</h2>
    <nuxt-link to="/">Home page</nuxt-link>
  </div>
</template>

<script>
export default {
  // もしバリデーションのメソッドが true または true に解決する Promise を返さない、またはエラーをスローした場合は、Nuxt.js は自動的に 404 エラーページあるいはエラーの場合 500 エラーページをロードします。
  validate({ params }) {
    return /^\d+$/.test(params.id) // 数値でなければならない
  }
}
</script>
