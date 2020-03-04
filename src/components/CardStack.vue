<template>
    <section class="card-stack">
        <Card 
        v-for="card in cards"
        :key="card.id"
        :card="card"
        @:click.native="emitCardId(card.id)"/>
    </section>
</template>
<script>
import Card from './Card'
export default {
    name: 'CardStack',
    components: {
        Card
        },
    props: {
        cards: Array
    },
    methods: {
        emitCardId(id) {
            this.$emit('emitId', id)
        }
    } 
}
</script>