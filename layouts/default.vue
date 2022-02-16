<template>
  <v-app >
    <header class="header">
      <div class="logo">
        <svg viewBox="0 0 57.692 35.546">
          <g transform="translate(-56.6 -611.8)">
            <path d="M562.149,646.626a5.3,5.3,0,0,1-7.233-1.937l-12.688-21.976-1.725-2.981q-.33-.621-.7-1.215a19.506,19.506,0,0,0-1.739-2.357,15.4,15.4,0,0,0-5.362-4.36h.5l11.893.008h.006a5.3,5.3,0,0,1,4.59,2.647l14.4,24.935A5.3,5.3,0,0,1,562.149,646.626Z" transform="translate(-466.574)" fill="#051dde"/>
            <path d="M1713.629,647.6h0a5.294,5.294,0,0,1-7.233-1.939l-14.391-24.923a5.294,5.294,0,0,1,1.939-7.233h0a5.294,5.294,0,0,1,7.233,1.939l14.391,24.923A5.294,5.294,0,0,1,1713.629,647.6Z" transform="translate(-1601.986 -0.975)" fill="#051dde"/>
              <g transform="translate(56.6 611.8)">
                <path d="M61.894,647.344h0A5.3,5.3,0,0,1,56.6,642.05V617.094a5.3,5.3,0,0,1,5.294-5.294h0a5.3,5.3,0,0,1,5.294,5.294v24.957A5.292,5.292,0,0,1,61.894,647.344Z" transform="translate(-56.6 -611.8)" fill="#01044e"/>
                <circle cx="5.282" cy="5.282" r="5.282" transform="translate(10.589 24.981)" fill="#01044e"/>
              </g>
            </g>
        </svg>
        <p>
          DuoMarkets
        </p>
      </div>
      <a v-for="btn in nav.btn_links" :key="btn.name" class="navbtn btn" :href="btn.link">
        {{ btn.name }}
      </a>
      <a href="" class="navbtn btn btn_border">Log In</a>
      <a href="" class="navbtn btn btn_filled">Sign Up</a>
    </header>
    <v-main>
      <!-- <v-container> -->
        <Nuxt />
      <!-- </v-container> -->
    </v-main>

    <v-footer class="footer" >
      <div class="ftr_navigation">
        <div class="col">
          <svg viewBox="0 0 73 48.221"><rect width="12.964" height="43.517" rx="6.482" transform="translate(0 2.343)" fill="#fff"/><path d="M568.9,654.407a6.482,6.482,0,0,1-8.855-2.372l-15.532-26.9-2.111-3.651q-.4-.761-.86-1.487a23.908,23.908,0,0,0-2.127-2.885c-1.846-2.146-4.215-4.434-6.564-5.337h.609l14.56.01h.008a6.479,6.479,0,0,1,5.619,3.242l17.625,30.528A6.481,6.481,0,0,1,568.9,654.407Z" transform="translate(-521.186 -609.429)" fill="#fff"/><rect width="12.964" height="48.196" rx="6.482" transform="translate(37.675 6.482) rotate(-30)" fill="#fff"/><circle cx="6.466" cy="6.466" r="6.466" transform="translate(12.964 32.927)" fill="#fff"/></svg>
        </div>
        <div class="col">
          <a v-for="btn in nav.btn_links.slice(0,3)" :key="btn.name" class="btn link" :href="btn.link">
            {{ btn.name }}
          </a>
        </div>
        <div class="col">
          <a v-for="btn in nav.btn_links.slice(3,6)" :key="btn.name" class="btn link" :href="btn.link">
            {{ btn.name }}
          </a>
        </div>
      </div>
      <div class="ftr_interactive">
        <div class="download">
          <button href="#" class="dwld_btn btn btn_border_white">
            <svg viewBox="0 0 27.312 32.781">
              <g transform="translate(-6.748 -4.5)">
                <path d="M27.028,10.821c-2.868,0-4.079,1.408-6.076,1.408-2.048,0-3.61-1.4-6.094-1.4A8.279,8.279,0,0,0,8.184,14.96c-2.313,3.67-1.92,10.583,1.826,16.471,1.34,2.108,3.132,4.472,5.479,4.5h.043c2.04,0,2.646-1.374,5.453-1.391h.043c2.765,0,3.32,1.383,5.351,1.383h.043c2.347-.026,4.233-2.646,5.573-4.745A23.344,23.344,0,0,0,34.06,27.2c-5.419-2.117-6.29-10.019-.93-13.049a8.025,8.025,0,0,0-6.1-3.328Z" transform="translate(0 1.351)" fill="#fff"/>
                <path d="M24.086,4.5a7.463,7.463,0,0,0-4.865,2.7,6.788,6.788,0,0,0-1.587,5.189h.137a6.335,6.335,0,0,0,4.762-2.569A7.269,7.269,0,0,0,24.086,4.5Z" transform="translate(2.311 0)" fill="#fff"/>
              </g>
            </svg>
            <!-- <p> -->
              App Store
            <!-- </p> -->
          </button>
          <button href="#" class="dwld_btn btn btn_border_white">
            <svg viewBox="0 0 28.779 31.925">
              <path d="M20.489,14.612,6.725.811,24.237,10.864l-3.748,3.748ZM3.132,0A2.424,2.424,0,0,0,1.779,2.2V29.723a2.424,2.424,0,0,0,1.353,2.2l16-15.966ZM29.65,14.07l-3.673-2.127-4.1,4.023,4.1,4.023,3.748-2.127a2.5,2.5,0,0,0-.075-3.792ZM6.725,31.12,24.237,21.067l-3.748-3.748Z" transform="translate(-1.779)" fill="#fff"/>
            </svg>
            <!-- <p> -->
              Play Store
            <!-- </p> -->
          </button>
        </div>
        <div class="subscribe">
          <p class="inf">
            Stay up to date with our Newsletter
          </p>
          <form class="form">
            <v-text-field
              placeholder="Enter your e-mail"
              filled
              rounded
              dense
              dark
              background-color="#01044E"
              color="#ffffff"
              height="40"
              :rules="rules"

            />
            <button class="form_btn btn_filled">
              Subscribe
            </button>
          </form>
        </div>
      </div>
      <div class="ftr_info">
        <p v-for="info in footer.infoBlock" :key="info" class="text" >{{ info }}</p>
      </div>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      rules: [
      value => !!value || 'Required.',
      value => {
        const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
       return pattern.test(value)|| 'Invalid e-mail'
      },
    ],
     nav:
     {
       btn_links:
       [
         {
           name: 'Home',
           link: '#'
         },
         {
           name: 'Platform',
           link: '#'
         },
         {
           name: 'Markets',
           link: '#'
         },
         {
           name: 'Tools',
           link: '#'
         },
         {
           name: 'Company',
           link: '#'
         },
         {
           name: 'Policies',
           link: '#'
         }
       ]
     },
     footer:{
       infoBlock:['© 2022 All rights reserved', '| ', 'Terms Of Service','| ', 'Privacy Policy','| ', 'Cookies']
     }
    }
  }
}
</script>

<style lang="scss" scoped>
@font-face {
    font-family: 'Helvetica Neue';
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueBlackCondensed.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueBoldCondensed.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Black.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-BlackItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Bold.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-BoldItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Heavy.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-HeavyItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Italic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Light.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-LightItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Medium.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-MediumItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Regular.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-Thin.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-ThinItalic.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-UltraLight.ttf") format('truetype');
    src: url("~/assets/fonts/Helvetica Neue/HelveticaNeueCyr-UltraLightItalic.ttf") format('truetype');
}

  .v-application--wrap{
    font-family: 'Helvetica Neue', sans-serif;
  }
  .header{
    position: fixed;
    width: 1140/1920*100vw;
    top: 40px;
    left: 50%;
    transform: translateX(-50%);
    @include makeitflex(row, space-between);
    z-index: 1000;
    .logo{
      display: flex;
      align-items: center;
      >p{
        font-size: $fs-24;
        color: $clr-blue;
        font-weight: bold;
      }
      >svg{
        height: 35/1920*100vw;
        width: auto;
        margin-right: 10px;
      }
    }
    .navbtn{
      font-size: $fs-18;
      font-weight: normal;
      align-self: center;
    }
  }

  .footer{
    @include makeitflex(column, flex-start);
    background-color: $clr-blue;
    padding: 60/1920*100vw 150/1920*100vw 45/1920*100vw;
    margin-top: auto;
    align-items: normal;
    .ftr_navigation{
      @include makeitflex(row,flex-start);

      .col{
        @include makeitflex(column, flex-start);
        margin-right: 120/1920*100vw;
        flex: 0;
        >svg{
          width: 73/1920*100vw;
          height: auto;
        }
        .link{
          color: $clr-white;
          font-size: $fs-18;
          font-weight: 400;
          margin-bottom: 25/1920*100vw;
        }
      }
    }
    .ftr_interactive{
      @include makeitflex(row, space-between);
      margin-bottom: 30/1920*100vw;
      .download{
          @include makeitflex(row,flex-start);
          align-items: flex-end;
        .dwld_btn{
          height: fit-content;
          font-size: $fs-20;
          padding: 15/1920*100vw;
          @include makeitflex(row,flex-start);
          align-items: center;
          flex: 1 1 0;
          margin-right: 30/1920*100vw;
            white-space: nowrap;
          >svg{
            height: 32/1920*100vw;
            width: auto;
            margin-right: 18/1920*100vw;
          }
          >p{
            white-space: nowrap;
          }
        }
      }
      .subscribe{
        .inf{
          font-size: $fs-18;
          font-weight: 400;
          color: $clr-white;
          margin-bottom: 25/1920*100vw;
        }
        .form{
          width: 460/1920*100vw;
          position: relative;
          .form_btn{
            font-size: $fs-18;
            position: absolute;
            padding: auto 42/1920*100vw;
            height: 30px;
            top: 0;
            right: 0;
            transform: translate(-5px, 5px)
          }
          .v-input{
            font-size: $fs-18 !important;
            & .v-input__control .v-text-field__details {
              position: absolute;
              right: 100%;
              width: fit-content;
              top: 50%;
              transform: translateY(-50%);
            }
          }

        }
      }
    }
    .ftr_info{
      @include makeitflex(row,flex-start);
      >p{
        margin-right: 5/1920*100vw;
        width: fit-content;
        font-size: $fs-18;
        color: $clr-white;
      }
    }
  }

</style>
