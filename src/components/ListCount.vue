<script>
import { store } from '../store';
    export default {
        name: 'counter',
        data(){
            return{
                store
            }
        }
    }
</script>

<template>
    <div class="mx-5 counter">
Risultati trovati : {{ store.charactersFound }}
    </div>
</template>


<style lang="scss">
.counter{
    padding: 15px 0px;
    background-color: black;
    color: white;
}
</style>