<template>
    <div class="time-when-used-container">
        <span class="time-when-used-text">or</span>
        <div>
          <input type="text">
          <i class="fa fa-info-circle tooltip" aria-hidden="true">
            <span class="tooltiptext">Press enter after typing the time.</span>
          </i>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.time-when-used-text {
    font-size: 0.8em;
    color: #fff;
    padding: 8px;
    text-shadow: 1px 1px #c50404;
    margin-right: auto;
}

.time-when-used-container {
  display: flex;
  flex-direction: column;
}

input {
    width: 20%;
    margin-right: 10px;
}

.tooltip {
  position: relative;
  margin-right: 10px;
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