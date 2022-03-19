<template>
    <v-container>
        <v-text-field
            label="Player 1*"            
            v-model="players[0]"
            :rules="[players[0] !== undefined, players[0] !== '']"
            autofocus
            class="danger"
        ></v-text-field>
        <v-text-field
            label="Player 2*"
            v-model="players[1]"
            :rules="[players[1] !== undefined, players[1] !== '']"
        ></v-text-field>
        <v-text-field
            label="Player 3*"
            v-model="players[2]"
            :rules="[players[2] !== undefined, players[2] !== '']"
        ></v-text-field>
        <v-text-field
            label="Player 4*"
            v-model="players[3]"
            :rules="[players[3] !== undefined, players[3] !== '']"
        ></v-text-field>
        <v-spacer></v-spacer>
        <v-btn
            block
            color="accent"
            elevation="2"
            v-on:click="showAlert()"
        >Start</v-btn>
    </v-container>
</template>

<script>
  export default {
    name: 'ContestantSignUp',
    data: () => ({
        players:[]
    }),
    methods:{
        showAlert: function(){
            alert(this.players[0]);
        }
    }
  }
</script>
