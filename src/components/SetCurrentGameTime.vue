<template>
    <div class="set-current-game-time">
        <span class="set-current-game-time-text">SET CURRENT GAME TIME</span>
        <div class="set-game-time-input-container">
            <input class="game-time-input" type="text">
            <i class="fa fa-info-circle tooltip" aria-hidden="true">
            <span class="tooltip-game-time">
                <span>Press enter after typing the time.<br></span>
                <span style="color: red">You only need to do this once.</span>
            </span>
            </i>    
        </div>      
        
    </div>
</template>

<script>
export default {

}
</script>

<style>
.set-current-game-time {
    align-self: center;
    display: flex;
    flex-direction: column;
}
.set-current-game-time-text {
    font-size: 1.5em;
    color: #fff;
    padding: 12px;
    text-shadow: 1px 1px #c50404;
}

.set-game-time-input-container {
    align-self: center;
}

.tooltip {
  position: relative;
}

.tooltip .tooltip-game-time {
  visibility: hidden;
  width: 210px;
  background-color: black;
  color: #fff;
  text-align: center;
  font-size: 0.8em;
  border-radius: 6px;
  padding: 5px 0;
  
  position: absolute;
  z-index: 1;
  top: 100%;
  left: 50%;
  margin-left: -60px;
}

.tooltip:hover .tooltip-game-time {
  visibility: visible;
}

.game-time-input {
    width: 50px;
}
</style>