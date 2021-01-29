<template>
    <div class="container">
        <div class="columns is-centered">
            <div class="column centered is-half">
                <figure class="image pic-size">
                    <img class="is-rounded" src="../assets/images/profilepic.png" alt="pic">
                </figure>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup () {
        

        return {}
    }
})
</script>

<style lang="scss" scoped>
    .pic-size {
        width: 104px;
        height: 104px;
    }
</style>