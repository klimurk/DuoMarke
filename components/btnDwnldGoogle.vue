<template>
  <a
  :href="link"
  class="dwld_btn btn"
  :class="{ btn_white:color=='white', btn_grey:color=='grey' }"
  >
    <svg viewBox="0 0 28.779 31.925">
      <path d="M20.489,14.612,6.725.811,24.237,10.864l-3.748,3.748ZM3.132,0A2.424,2.424,0,0,0,1.779,2.2V29.723a2.424,2.424,0,0,0,1.353,2.2l16-15.966ZM29.65,14.07l-3.673-2.127-4.1,4.023,4.1,4.023,3.748-2.127a2.5,2.5,0,0,0-.075-3.792ZM6.725,31.12,24.237,21.067l-3.748-3.748Z" transform="translate(-1.779)" />
    </svg>
    Play Store
  </a>
</template>

<script>
export default {
  name: 'BtnDwnldPlayStore',
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
    height: fit-content;
    font-size: $fs-20;
    padding: 15/1920*100vw;
    @include makeitflex(row,flex-start);
    align-items: center;
    margin-right: 30/1920*100vw;
    white-space: nowrap;
    // padding: 10/1920*100vw 23/1920*100vw;
    border-radius:10/1920*100vw;
    align-items: center;
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
