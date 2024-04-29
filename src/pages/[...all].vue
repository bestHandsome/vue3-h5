<!--
 * @Author: xingjin
 * @Date: 2024-03-18 16:48:46
 * @LastEditors: xingjinjin
 * @LastEditTime: 2024-04-29 14:27:57
 * @Description: 请填写简介
-->
<script lang="ts" setup>
onMounted(() => {
  const canvas = document.getElementById('myCanvas')
  const ctx = canvas.getContext('2d')
  const img = new Image()

  img.src = 'http://zheshang.anjijin.org:8808/assets/png/login_map-11da9bb5.png'
  img.onload = function () {
    ctx.drawImage(img, 0, 0, 300, 300)
    ctx.save()
    ctx.font = '12px Arial'
    ctx.fillText('Hello World', 150, 100)
    ctx.restore()
  }
})
</script>

<template>
  <div>
    Not found
  </div>
  <img id="picture" src="/pwa-192x192.png" alt="">
  <p class="text-blue">
    111
  </p>
  <canvas id="myCanvas" width="300" height="300" />
</template>

<route lang="yaml">
meta:
  layout: 404
</route>
