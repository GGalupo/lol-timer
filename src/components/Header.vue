<template>
    <header class="header">
        <img class="logo" src="../assets/logo.png" alt="Logo">
        <SetCurrentGameTime />
        <CurrentGameTime />
        <img class="back-to-menu" src="../assets/imgs/back.png" alt="Back to the menu arrow">
    </header>
</template>

<script>
import CurrentGameTime from './CurrentGameTime'
import SetCurrentGameTime from './SetCurrentGameTime'

export default {
    components: {
        CurrentGameTime,
        SetCurrentGameTime
    }
}
</script>

<style>
.header {
    grid-area: header;
    display: flex;
}

.back-to-menu {
    /* position: absolute;
    top: 15px;
    right: 15px;
    width: 40px; */
    margin-left: auto;
    align-self: center;
    width: 40px;
    margin-right: 15px;
}

.logo {
    align-self: center;
    margin-right: auto;
    margin-left: 25px;
    width: 70px;
}

.back-to-menu:hover {
    opacity: 0.4;
    cursor: pointer;
}

.back-to-menu:active {
    position:relative;
	top:1px;
}
</style>