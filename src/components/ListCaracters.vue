<script>
import axios from 'axios';
import CartaCard from './CartaCard.vue';
import { store } from '../store';

export default {
    name: 'list',
    components: {
        CartaCard,
       
    },
    data() {
        return {
            store,
            characters: []
        }
    },
    created() {
                    axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php')
                .then((Response) => {
                    console.log(Response)
                    this.store.characters = Response.data.data;
                    this.store.charactersFound = Response.data.data.length;
                })
        }}

</script>
<template>
    <div class="container">
        <div class="row g-3">
            <div class="row-cols-12 col-sm-5" v-for="character in store.characters">
                <CartaCard :img="character.card_images[0].image_url"  :title="character.name" :type="character.type" />
            </div>
        </div>
    </div>
</template>



<style lang="scss" >



</style>