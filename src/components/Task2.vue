<template>
    <div id="t2-main">
        <div class="inner" id="t2--1">
            <v-btn variant="tonal">
                Button
            </v-btn>
        </div>
        <div class="inner" id="t2--2">
            <v-card variant="outlined">
                <v-card-text>
                    Top Left Text
                </v-card-text>
            </v-card>
            <v-card variant="outlined" class="bottom-right">
                <v-card-text>
                    Bottom Right Text
                </v-card-text>
            </v-card>
        </div>
        <div class="inner" id="t2--3">
            <v-card variant="outlined" class="top-right">
                <v-card-text>
                    Top Right Text
                </v-card-text>
            </v-card>
            <v-card variant="outlined" class="bottom-right">
                <v-card-text>
                    Bottom Right Text
                </v-card-text>
            </v-card>
        </div>
    </div>
</template>

<style scoped>
    #t2-main {
        height: 100%;
        width: 100%;
    }

    .inner {
        height: 33%;
        text-align: none;
    }

    #t2--1 {
        text-align: left;
    }

    #t2--1 button{
        width: 33%;
        height: 33%;
    }

    #t2--2 {
        background-color: darkgray;
        position: relative;
    }
    #t2--2 .v-card {
        width: 33%;
        height: 33%;
    }

    #t2--2 .bottom-right{
        position: absolute;
        bottom: 0;
        right: 0;
    }

    #t2--3 {
        position: relative;
    }

    #t2--3 .v-card {
        height: 33%;
        width: 33%;
    }

    #t2--3 .top-right {
        position: absolute;
        top: 0;
        right: 0;
    }

    #t2--3 .bottom-right{
        position: absolute;
        right: 0;
        bottom: 0;
    }
</style>