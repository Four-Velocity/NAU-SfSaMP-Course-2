<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
    width="400"
    height="200"
  >
    <template v-for="index in 11" :key="index">
      <rect
        width="100%"
        height="18.18"
        :y="18.18 * (index - 1)"
        :fill="index % 2 === 1 ? '#EF3340' : '#FFFFFF'"
      ></rect>
    </template>

    <rect width="22.725%" height="45.45%" y="0" fill="#00205B"></rect>

    <g transform="translate(45,45) scale(25)">
      <g id="B">
        <polygon
          id="A"
          fill="#fff"
          points="0,0 0,1 .5,1"
          transform="translate(0,-1) rotate(18)"
        />
        <use xlink:href="#A" transform="scale(-1,1)" />
      </g>
      <g id="C">
        <use xlink:href="#B" transform="rotate(72)" />
        <use xlink:href="#B" transform="rotate(216)" />
      </g>
      <use xlink:href="#C" transform="rotate(72)" />
    </g>
  </svg>
</template>
<style scoped>
svg {
  margin-top: 35px;
}
</style>