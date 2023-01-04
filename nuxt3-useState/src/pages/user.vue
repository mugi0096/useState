<script lang="ts" setup>
const user = useState<{ id: string, name: string, mail: string }>('login-user', () => {
  console.log('retrieving user info...');
  return {
    id: '123',
    name: 'ueno',
    mail: 'test@example.com'
  };
})
</script>

<template>
  <div>
    <h1>useState実装例</h1>
    <nuxt-link to="/user-detail">{{ user.name }}さんの詳細ページ</nuxt-link>
  </div>
</template>