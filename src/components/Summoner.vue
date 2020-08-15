<template>
    <div class="summoner-card">
        <Champion />
        <div class="timer-changers">
            <Cdr src="UnsealedSpellbook.png" />
            <Cdr src="CosmicInsight.png" />
            <Cdr src="3158.png" />
        </div>
        <Informations />
        <hr>
        <Informations />
    </div>
</template>

<script>
import Champion from './Champion'
import Informations from './Informations'
import Cdr from './CDR'

export default {
    components: {
        Champion,
        Informations,
        Cdr
    }
}
</script>

<style>
.summoner-card {
    border: 2px solid rgba(0, 0, 0, 0.473);
    width: 20%;
    margin: 15px;
    box-shadow: 10px 5px 5px black;
    max-width: 380px;

    /* background: linear-gradient(to right, #FFEFBA, #FFFFFF); */
}

.timer-changers {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-left: 15px;
    padding-right: 15px;
}
</style>