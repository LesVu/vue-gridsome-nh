<template>
  <v-app>
    <v-app-bar color="teal lighten-3" dense elevation="1" rounded app>
      <v-app-bar-nav-icon />
      <v-app-bar-title
        ><g-link to="/" class="text-decoration-none"><span></span></g-link
      ></v-app-bar-title>
      <v-spacer />
      <g-link to="/all" class="text-decoration-none"
        ><v-btn color="accent" elevation="4">All</v-btn>
      </g-link>
    </v-app-bar>
    <slot />
  </v-app>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
