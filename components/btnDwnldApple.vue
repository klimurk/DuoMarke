<template>
  <a
  :href="link"
  class="dwld_btn btn"
  :class="{ btn_white:color=='white', btn_grey:color=='grey' }"
  >
    <svg viewBox="0 0 27.312 32.781">
      <g transform="translate(-6.748 -4.5)">
        <path d="M27.028,10.821c-2.868,0-4.079,1.408-6.076,1.408-2.048,0-3.61-1.4-6.094-1.4A8.279,8.279,0,0,0,8.184,14.96c-2.313,3.67-1.92,10.583,1.826,16.471,1.34,2.108,3.132,4.472,5.479,4.5h.043c2.04,0,2.646-1.374,5.453-1.391h.043c2.765,0,3.32,1.383,5.351,1.383h.043c2.347-.026,4.233-2.646,5.573-4.745A23.344,23.344,0,0,0,34.06,27.2c-5.419-2.117-6.29-10.019-.93-13.049a8.025,8.025,0,0,0-6.1-3.328Z" transform="translate(0 1.351)" />
        <path d="M24.086,4.5a7.463,7.463,0,0,0-4.865,2.7,6.788,6.788,0,0,0-1.587,5.189h.137a6.335,6.335,0,0,0,4.762-2.569A7.269,7.269,0,0,0,24.086,4.5Z" transform="translate(2.311 0)" />
      </g>
    </svg>
      App Store
  </a>
</template>

<script>
export default {
  name: 'BtnDwnldAppStore',
  props: {
    color: {
      type: String,
      default: 'white',
      require: true
    },
    link: {
      type: String,
      default: '#',
      require: true
    }
  }
}
</script>

<style lang="scss" scope>
  .dwld_btn{
    text-decoration: none;
    height: fit-content;
    font-size: $fs-20;
    padding: 15/1920*100vw;
    @include makeitflex(row,flex-start);
    align-items: center;
    width: fit-content;
    margin-right: 30/1920*100vw;
    white-space: nowrap;
    align-items: center;
    // padding: 10/1920*100vw 23/1920*100vw;
    border-radius:10/1920*100vw;
    >svg{
      height: 32/1920*100vw;
      width: auto;
      margin-right: 18/1920*100vw;
    }
    >p{
      white-space: nowrap;
    }
  }
.btn_white{
  border: $clr-white 2px solid;
  color: $clr-white !important;
  fill: $clr-white;
}
.btn_grey{
  border: $clr-grey-light 2px solid;
  color: $clr-grey-dark !important;
  fill: $clr-grey-dark;
}

</style>
