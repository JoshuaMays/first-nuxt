<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
const DIGIT_REGEX = /^\d+$/;

export default {
  validate(data) {
    return DIGIT_REGEX.test(data.params.id);
  },
  layout: 'users'
}
</script>
