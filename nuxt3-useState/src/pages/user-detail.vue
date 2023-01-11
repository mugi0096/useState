<script lang="ts" setup>
import type { Ref } from 'vue';

type User = {
  id: string;
  name: string;
  mail: string;
};

const user: Ref<User> = useState('login-user')
</script>

<template>
  <div>
    <p>ユーザーID: {{ user.id }}</p>
    <p>ユーザー名: {{ user.name }}</p>
    <p>メールアドレス: {{ user.mail }}</p>
  </div>
</template>