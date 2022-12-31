<template>
    <v-card 
        tile 
        flat 
        rounded="lg"
        class="pa-md-10 pa-5 text-center" 
        color="surface" >
        <h2 class="text-md-h6 font-weight-bold">FreeCommerce</h2>
        <p class="text-md-body-2 mt-5">Free eCommerce Site Built With NuxtJS ❤</p>
        <div class="text-center">
            <v-btn 
                v-for="(b, i) in sm" 
                :key="`socialMedia-${i}`" 
                color="surface" 
                class="mr-2" 
                fab 
                depressed>
                <v-icon>{{b.icon}}</v-icon>
            </v-btn>
        </div>
    </v-card>
</template>

<script>
    export default{
        data(){
            return{
                sm:[
                    {
                        icon:'mdi-facebook',
                        link:'http://www.facebook.com',
                    },
                    {
                        icon:'mdi-whatsapp',
                        link:'http://www.wathsapp.com',
                    },
                    {
                        icon:'mdi-instagram',
                        link:'http://www.instagram.com',
                    },
                    {
                        icon:'mdi-twitter',
                        link:'http://www.twitter.com',
                    },
                    {
                        icon:'mdi-youtube',
                        link:'http://www.youtube.com',
                    },
                ]
            }
        }
    }
</script>