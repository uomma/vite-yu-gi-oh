<script >
import ListCaracters from './ListCaracters.vue';
export default{
    name: 'main',
    components: {
       ListCaracters,
    }
}
</script>

<template>
   
        <main class="mx-5">
            <div class="dropdown my-5">
                <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Dropdown button
                </button>
                <ul class="dropdown-menu">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                </ul>
            </div>
            <ListCaracters/>
        </main>
 
</template>



<style lang="scss" scoped>

</style>