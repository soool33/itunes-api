<template>
    <div
    id="e3"
    style="max-width: 400px; margin: auto"
    class="grey lighten-3"
    >
        <v-container
        fluid
        style="min-heught: 0;"
        grid-list-lg
        >
            <v-layout row wrap>
                <v-flex xs12>
                    <v-card target="_blank" :href="url" :color="color" class="white--text">
                        <v-card-title primary-title>
                            <div>
                                <div class="headline">{{title}}</div>
                                <span>{{artistName}}</span>
                            </div>
                        </v-card-title>
                        <v-card-media
                        :src="image"
                        height="100px"
                        contain
                        >
<!--                            <v-btn flat dark>Listen now</v-btn>-->
                        </v-card-media>
                    </v-card>
                </v-flex>
            </v-layout>
        </v-container>


    </div>
</template>

<script>
    export default {
        props: ['title','image','artistName','url','color']
    }

</script>
