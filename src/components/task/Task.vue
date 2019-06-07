<template>
    <v-expansion-panel-content>
        <template v-slot:header>
            <v-flex xs2>
                <v-avatar >
                    <span class="white-text">#{{ id }}</span>
                </v-avatar>
            </v-flex>
            <div> {{ title }} </div>
        </template>
        <v-card>
            <v-card-text>
                {{ content }}
            </v-card-text>
        </v-card>
    </v-expansion-panel-content>

</template>

<script>
export default {
    name: 'Task',
    components:{
    },
    props: [
        'title',
        'id',
        'content'
        ]
}
</script>

<style>

</style>
