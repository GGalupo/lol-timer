<template>
    <div class="informations">
        <Spell />
        <div class="buttons-container">
            <Button label="5s" />
            <Button label="10s" />
            <Button label="15s" />
        </div>
        <Timers />
        <TimeWhenWasUsed />
    </div>
</template>

<script>
import Button from './Button'
import Spell from './Spell'
import Timers from './Timers'
import TimeWhenWasUsed from './TimeWhenWasUsed'
export default {
    components: {
        Spell,
        Timers,
        TimeWhenWasUsed,
        Button
    }
}
</script>

<style>
.buttons-container {
    display: flex;
    justify-content: space-around;
    margin: 7px;
}

.informations {
    height: 100%;
}
</style>