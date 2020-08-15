<template>
    <div class="time-when-used-container">
        <div class="time-when-used-text">or game time when used</div>
        <input type="text">
        <i class="fa fa-info-circle tooltip" aria-hidden="true">
            <span class="tooltiptext">Press enter after typing the time.</span>
        </i>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.time-when-used-text {
    font-size: 0.7em;
    color: #fff;
    padding: 13px 5px;
    text-shadow: 1px 1px #c50404;
}

.time-when-used-container {
    display: flex;
    justify-content: space-around;
    align-items: center;
}

input {
    width: 20%;
    margin-right: 10px;
}

.tooltip {
  position: relative;
  display: inline-block;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  font-size: 0.7em;
  border-radius: 6px;
  padding: 5px 0;
  
  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  bottom: 100%;
  left: 50%;
  margin-left: -120px;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>