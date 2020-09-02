<template>
  <footer class="footer">
    <div class="last-update">
      Last update: <span style="color: orange">Patch 10.16</span>
    </div>
    <CopyTimes />
    <div class="developer-info">
      <span class="developer">Developed by Gustavo <span style="color: red">Galupo</span></span>
      <a href="https://instagram.com/ggalupo" target="_blank">
          <i class="fa fa-instagram"></i>
      </a>
      <a href="https://github.com/GGalupo" target="_blank">
            <i class="fa fa-github"></i>
      </a>
    </div>
  </footer>
</template>

<script>
import CopyTimes from './CopyTimes'
export default {
  components: {
    CopyTimes
  }
}
</script>

<style>
.footer {
    grid-area: footer;

    display: flex;
    align-items: center;
    color: #fff;
}

.last-update {
  margin-right: auto;
  padding: 15px;
}

.developer-info {
  margin-left: auto;
}

.developer {
  margin-right: 6px;
}

a i {
  margin: 0 8px;
  color: black;
}

a i:hover {
  cursor: pointer;
  opacity: 0.6;
}
</style>