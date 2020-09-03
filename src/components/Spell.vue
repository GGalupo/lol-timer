<template>
    <div class="spell-container">
        <img class="spell" src="../assets/imgs/SummonerFlash.png" alt="">
        <i class="fa fa-info-circle tooltip" aria-hidden="true">
            <span class="tooltiptext">Choose the time since the spell was used.</span>
        </i>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.spell {
    width: 15%;
    margin: 10px;
    border: 2px solid black;
    box-shadow: 3.5px 2px 2px black;
}

.spell-container {
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>