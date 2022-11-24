<template>
    <div>
        <div class="prodotti">
            <h1>SCOPRI TUTTI I <strong>PRODOTTI</strong></h1>
            <h2>Scopri la <strong>pasta La Molisana:</strong> tipi di pasta da grano 100% italiano decorticato e
                trafilata al bronzo</h2>
        </div>
        <div class="pre-pasta">
            <i class="fa-regular fa-square"></i>
            <span class="pastatext">Pasta per <strong>forma</strong></span>
        </div>
        <div class="Pasta-card-Div-Flex">
            <PastaCard v-for="(element, index) in arrayPasta" :key="index" :propsPasta="element"/>
        </div>
    </div>
</template>


<script>
import PastaCard from './PastaCard.vue'

export default {
    name: 'MainComp',
    components: {
        PastaCard
    },
    data() {
        return {
            arrayPasta: [
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/03/1-spaghetto-quadrato-2.png",
                    'tipo': 'Pasta Lunga'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/29-caserecce-molisane.png",
                    'tipo': 'Pasta Corta'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/03/15-spaghetti-1.png",
                    'tipo': 'Spaghetti'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/20-penne-rigate.png",
                    'tipo': 'Penne'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2022/01/28-fusilli.png",
                    'tipo': 'Fusilli'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/ziti-tagliati.webp",
                    'tipo': 'Ziti'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/10/gnocchi.png",
                    'tipo': 'Gnocchi'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/10/50-ditalini-rigati-grandi-cucine.png",
                    'tipo': 'Ditali'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2022/04/pastina.webp",
                    'tipo': 'Pastina'
                },

            ]
        }
    }

}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.prodotti {
    width: 80%;
    display: flex;
    justify-content: space-between;
    margin: 5px auto;
}

h1 {
    flex-basis: 50%;
    font-weight: normal;
}

h2 {
    font-style: italic;
    font-weight: normal;
}

.pastatext {
    font-style: italic;
}

.pre-pasta {
    width: 80%;
    margin: 30px auto;
    font-size: 1.8rem;
}

.fa-square {
    color: orange;
    padding: 5px 5px;
}

.Pasta-card-Div-Flex {
    display: flex;
    width: 80%;
    flex-wrap: wrap;
}
</style>