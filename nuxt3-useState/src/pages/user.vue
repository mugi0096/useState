<script lang="ts" setup>
type User = {
  id: string;
  name: string;
  mail: string;
};

const user = useState<User>('login-user', () => {
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