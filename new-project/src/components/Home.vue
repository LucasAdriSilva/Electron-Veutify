<template>
    <v-container fluid> 
        <v-forme>
            <v-file-input 
            label="Selecione as legendas"
            multiple 
            chips 
            v-model="files" />

           
        </v-forme>
        <div class="pills">
            <Pill v-for="word in grupedWord" :key="word.name" :name="word.name" :amount="word.amount"/>
        </div>
    </v-container>
</template>

<script>
import Pill from './Pill.vue'
export default {
    components:{
        Pill,
    },
    data: function (){
        return{
            files:[],
            grupedWord:[
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},
                {name: 'you', amount: 900},
                {name: 'i', amount: 6541},
                {name: 'she', amount: 645},

            ]
        }
    },
    methods:{
        processSubtitles(){
           console.log(this.files);
        }
    }
}
</script>

<style>
    .pills{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

</style>