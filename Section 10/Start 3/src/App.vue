<template>
    <div class="container">
        <app-new-quote @quoteAdded="newQoute"></app-new-quote>
        <app-quote-grid :quotes="quotes"></app-quote-grid>
        <div class="row">
            <div class="col">

            </div>
        </div>
    </div>
</template>

<script>
    import QuoteGrid from "./components/QuoteGrid.vue";
    import NewQuote from "./components/NewQuote.vue";
    
    export default {
        data: function () {
            return {
                maxQuotes: 10,
                quotes: [
                    'Just a Quote to see something'
                ]
            }
        },
        components: {
            "app-quote-grid": QuoteGrid,
            'app-new-quote': NewQuote
        },
        methods:{
            newQoute(qoute){
                this.quotes.push(qoute);
            }
        }
    }
</script>

<style>
</style>
