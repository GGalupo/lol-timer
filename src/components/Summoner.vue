<template>
    <div class="summoner-card">
        <Champion />
        <div class="timer-changers">
            <Cdr src="UnsealedSpellbook.png" />
            <Cdr src="CosmicInsight.png" />
            <Cdr src="3158.png" />
        </div>
        <Informations />
        <div class="divisor"></div>
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

    display: flex;
    flex-direction: column;

    /* background: linear-gradient(to right, #FFEFBA, #FFFFFF); */
}

.timer-changers {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0 15px;
    border-bottom: 1px solid rgb(202, 70, 70);
    border-top: 1px solid rgb(202, 70, 70);

    background: linear-gradient(to bottom, rgba(129, 48, 48, 0.836), #42275abb);
}

.divisor {
    width: 100%;
    background-color: rgb(202, 70, 70);
    height: 1px;
    margin: 5px 0;
}
</style>