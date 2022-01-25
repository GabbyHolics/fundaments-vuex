<template>
    <h1>  Vue Acces </h1>
    <h2>  Direct Access: {{ $store.state.count }} </h2>
    <h3> {{ count }} </h3>

</template>

<script>
import { mapState } from 'vuex'
export default {

    computed: {
        countComputed(){
        return console.log('hola')
    },
    ...mapState(['count'])
    }
}
</script>
