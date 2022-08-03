<template>
    <v-layout class="App">
        <Navigation msg="Dashboard" />
        <v-main>
            <v-container fluid>
                <v-row>
                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>

                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>

                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>

                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>

                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>

                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>


                    <v-col v-for="n in 4" :key="n" lg="3" md="6" sm="12" cols="12">
                        <v-card elevation="5" :title="`Content ${n}`" :subtitle="`Subtitle for Content ${n}`"
                            text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"></v-card>
                    </v-col>
                </v-row>
            </v-container>

        </v-main>
    </v-layout>
</template>

<script>
export default {

}
</script>

<style>
.App {
    font-family: 'Noto sans lao';
}
</style>