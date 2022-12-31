<template>
    <div>
        <v-app-bar 
            color="surface"
            height="80" 
            class="el" 
            app 
            :style="{padding : $vuetify.breakpoint.modAndUp ? '0px 100px' : '',}">
        <v-toolbar-title 
            class="text-md-h5 font-weight-bold pointer">
            FreeCommerce
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn nuxt to="/" class="mr-md-2" icon>
            <v-icon size="20">mdi-store-outline</v-icon>
        </v-btn>
        <v-badge
        
        >
        <v-btn nuxt to="/" icon>
            <v-icon size="20">mdi-cart-outline</v-icon>
        </v-btn>
        </v-badge>
        <v-btn icon>
            <v-icon size="20">mdi-cart-outline</v-icon>
        </v-btn>
        <v-divider vertical class="mx-md-5 mx-2"></v-divider>
        <v-btn @click="toggleTheme" icon>
            <v-icon size="20">mdi-brightness-8</v-icon>
        </v-btn>
        </v-app-bar>
    </div>
</template>

<script>
export default {
    methods: {
        toggleTheme() {
        this.$vuetify.theme.dark = !this.$vuetify.theme.dark;
        },
  },
}
</script>