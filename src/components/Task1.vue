<template>
    <div id="t1-main">
        <div class="inner" id="t1--1">
            <v-btn variant="tonal">
                Button
            </v-btn>
        </div>
        <div class="inner" id="t1--2">
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
        <div class="inner" id="t1--3">
            <v-card variant="outlined">
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
    #t1-main {
        height: 100%;
        width: 100vw;
        margin: 0;
        display: flex;
        flex-direction: column;
        align-items: stretch;
        justify-content: stretch;
    }
    .inner {
        flex: 1;
        display: flex;
        flex-direction: row;
        width: 100vw;
    }

    #t1--1 button{
        height: 33%;
        width: 33%;
    }

    #t1--2 {
        background-color: darkgray;
        justify-content: space-between;
    }

    #t1--2 .v-card{
        height: 33%;
        width: 33%;
    }

    #t1--2 .bottom-right {
        align-self: flex-end;
    }

    #t1--3 {
        flex-direction: column;
        gap: 34 %
    }

    #t1--3 .v-card {
        height: 33%;
        width: 33%;
        margin-left: auto;
        margin-right: 0;
    }

</style>