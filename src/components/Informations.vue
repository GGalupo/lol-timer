<template>
    <div>
        <div class="spell-info">
            <Spell />
            <SpellWasUsed />
        </div>
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
import SpellWasUsed from './SpellWasUsed'
import TimeWhenWasUsed from './TimeWhenWasUsed'
export default {
    components: {
        Spell,
        Timers,
        SpellWasUsed,
        TimeWhenWasUsed,
        Button
    }
}
</script>

<style>
.spell-info {
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
}

.buttons-container {
    display: flex;
    justify-content: space-around;
    margin: 7px;
}
</style>