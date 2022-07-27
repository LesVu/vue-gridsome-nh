<template>
<v-container>
      <v-app-bar color="blue" dense elevation="1" rounded>
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
      </v-app-bar>
    <slot/>
  </v-container>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>


