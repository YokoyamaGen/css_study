<template>
  <div class="gnav_draewr gnav_standard_icon section-name">
    <div class="section_inner">
      <!-- PC -->
      <nav class="gnav gnav_pc gnav_container gnav_text-color">
        <div class="gnav_bg gnav_bg-color" style="background-color: rgba(255, 255, 255, 0.9);"></div>
        <header class="logo_side">
          <div class="header_logo">
            <a data-href="/">
              <img src="//flamingo.eat.auto/section/images/sample_place_logo_bk.png" alt="logo">
            </a>
          </div>
        </header>
        <ul class="gnav_items">
          <li><a class="submenu-link" data-href="">事業内容</a>
            <ul class="dropdownSubMenu gnav_sub_bg-color" style="background-color: rgba(255, 255, 255, 0.9);">
              <li><a data-href="">事業内容1</a></li>
              <li><a data-href="">事業内容2</a></li>
              <li><a data-href="">事業内容3</a></li>
              <li><a data-href="">事業内容4</a></li>
              <li><a data-href="">事業内容5</a></li>
            </ul>
          </li>
          <li><a data-href="">求人情報</a></li>
          <li><a data-href="">ショーケース</a></li>
          <li><a data-href="">ブログ</a></li>
          <li><a data-href="">会社情報</a></li>
        </ul>

        <!-- content -->
        <div class="gnav-editable-contents gnav-right-groups">
          <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://www.instagram.com/"><img src="https://flamingo.eat.auto/section/images/place_ig_color.png"></a>
          <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://twitter.com/"><img src="https://flamingo.eat.auto/section/images/place_tw_color.png"></a>
          <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://facebook.com/"><img src="https://flamingo.eat.auto/section/images/place_fb_color.png"></a>
          <a class="gnav-icon" data-href="tel://0354141822"><img src="https://flamingo.eat.auto/section/images/place_tel_navyblue.png"></a>
          <a class="gnav-btn" data-href="/contact">お問い合わせ</a>
        </div>
      </nav>

      <!-- SP -->
      <nav class="gnav gnav_sp gnav_container gnav_text-color">
        <div class="hamburger-box">
          <input id="drawer-checkbox" type="checkbox">
          <label id="hamburger" class="hamburger" for="drawer-checkbox">
            <span class="hamburger_top drawer-hamburger-icon"></span>
            <span class="hamburger_mid drawer-hamburger-icon"></span>
            <span class="hamburger_btm drawer-hamburger-icon"></span>
          </label>

          <div class="gnav_bg gnav_bg-color" style="background-color: rgba(255, 255, 255, 0.9);"></div>
          <header class="logo_side">
            <div class="header_logo">
              <a data-href="/">
                <img src="//flamingo.eat.auto/section/images/sample_place_logo_bk.png" alt="logo">
              </a>
            </div>
          </header>
        </div>

        <div class="sidebar-box gnav_bg gnav_bg-color" style="background-color: rgba(255, 255, 255, 0.9);">
          <header class="logo_side">
            <div class="header_logo">
              <a data-href="/">
                <img src="//flamingo.eat.auto/section/images/sample_place_logo_bk.png" alt="logo">
              </a>
            </div>
          </header>
          <ul class="gnav_items">
            <li>
              <a class="submenu-link" data-href="">事業内容</a>
              <ul class="dropdownSubMenu">
                <li><a data-href="">事業内容1</a></li>
                <li><a data-href="">事業内容2</a></li>
                <li><a data-href="">事業内容3</a></li>
                <li><a data-href="">事業内容4</a></li>
                <li><a data-href="">事業内容5</a></li>
              </ul>
              <div class="open-icon"></div>
            </li>
            <li><a data-href="">求人情報</a></li>
            <li><a data-href="">ショーケース</a></li>
            <li><a data-href="">ブログ</a></li>
            <li><a data-href="">会社情報</a></li>
          </ul>

          <!-- content -->
          <div class="gnav-editable-contents gnav-right-groups">
            <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://www.instagram.com/"><img src="https://flamingo.eat.auto/section/images/place_ig_color.png"></a>
            <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://twitter.com/"><img src="https://flamingo.eat.auto/section/images/place_tw_color.png"></a>
            <a class="gnav-icon" target="_blank" rel="noreferrer" data-href="https://facebook.com/"><img src="https://flamingo.eat.auto/section/images/place_fb_color.png"></a>
            <a class="gnav-icon" data-href="tel://0354141822"><img src="https://flamingo.eat.auto/section/images/place_tel_navyblue.png"></a>
            <a class="gnav-btn" data-href="/contact">お問い合わせ</a>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
  import mixin from "./gnav-helpers"
  export default {
    mixins: [mixin],
    code: "gnav_standard_icon",
    name: "gnav_standard_icon",
    gnav_type: "accordion",
    gnav_contents: '{gn_content1: {"type":"icon", "image": "", "link":""}}',

    data() {
      return {
        js_urls: ["//flamingo.eat.auto/javascripts/sections/scroll_observe.min.js", "//flamingo.eat.auto/javascripts/sections/gnav_methods.js", "//flamingo.eat.auto/gnavs/gnav_accordion_block/gnav_accordion_block.js"],
        css_urls: ["//cms.localhost:3102/tmp_css/gnav_standard_icon.css"],
      }
    },

    mounted() {
      this.appendScripts(this.js_urls, this.css_urls)
    },

    methods: {

    }
  }
</script>

// コンテンツの定義
<contents>
[
  {"id": "gn_content1", "type": "icon", "pc_visible": true, "sp_visible": true, "image": "https://flamingo.eat.auto/section/images/place_ig_color.png", "link": "https://www.instagram.com/", "link_type": "external" },
  {"id": "gn_content2", "type": "icon", "pc_visible": true, "sp_visible": true, "image": "https://flamingo.eat.auto/section/images/place_tw_color.png", "link": "https://twitter.com/", "link_type": "external" },
  {"id": "gn_content3", "type": "icon", "pc_visible": true, "sp_visible": true, "image": "https://flamingo.eat.auto/section/images/place_fb_color.png", "link": "https://facebook.com/", "link_type": "external" },
  {"id": "gn_content4", "type": "icon", "pc_visible": true, "sp_visible": true, "image": "https://flamingo.eat.auto/section/images/place_tel_navyblue.png", "link": "0354141822", "link_type": "tel" },
  {"id": "gn_content5", "type": "btn", "pc_visible": true, "sp_visible": true, "text":"お問い合わせ", "link": "/contact", "link_type": "internal" }
]
</contents>

<style lang="scss">
// 共通設定
@import "../settings";
// 共通
// #global-nav {
//   width: 100%;
//   position: fixed;
//   top: 0;
//   left: 0;
//   transition: translateY .6s;
//   z-index: 5;
//   padding: 20px;
// }

.gnav_items{
  font-weight: bold;
  font-family: 游ゴシック体;
  letter-spacing: 0.08em;
}

#drawer-checkbox {
  display: none;
}

.gnav-editable-contents {
  .gnav-icon {
    margin: 10px 24px 8px 0;

    img {
      width: 30px;
      height: 30px;
      object-fit: contain;
    }
  }

  .gnav-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 120px;
    height: 40px;
    color: #FFF;
    background-color: #12BA8D;
    border-radius: 20px;
    font-size: 12px;
    line-height: initial;
    margin-left: 12px;
  }
}

// PC
@media #{$pc_style_min} {
  // menuオープン時のスクロールロック
  // html.scroll-locked {
  //   overflow: auto;
  // }

  #global-nav {
    // スクロールしたとき
    // &.smart {
    //   padding: 20px;
    //   transform: translateY(0);
    //   position: fixed;

    //   .gnav_standard_icon.gnav_draewr {
    //     padding: 0;
    //   }

      // .gnav_container {
      //   height: 100%;
      // }
    }
  }

  .gnav_container {
    // &.gnav_pc {
    //   #global-nav & {
    //     display: flex;
    //   }

    //   .gnav-editable-contents {
    //     align-items: center;
    //     position: absolute;
    //     right: 25px;
    //     display: flex;
    //     height: 100%;
    //   }
    // }

    &.gnav_sp {
      #global-nav & {
        display: none;
      }
    }
  }

  // .hamburger {
  //   display: none;
  // }
}

@keyframes SidebarSlideIn {
  0% {
    width: 0px;
  }
  100% {
    width: calc(100% - 90px);
  }
}
@keyframes IconFadeIn {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

// SP
@media #{$pc_style_max} {
  #global-nav {
    width: 100%;
    padding: 10px;
    position: fixed;
    top: 0;
    left: 0;
    transition: translateY .6s;
    z-index: 5;

    // .hamburger-box .gnav_bg {
    //   border-radius: 10px;
    // }
  }

  .gnav_container {
    &.gnav_pc {
      #global-nav & {
        display: none;
      }
    }

    &.gnav_sp {
      #global-nav & {
        display: block;
      }

      // .gnav-editable-contents {
      //   align-items: center;
      //   position: absolute;
      //   left: 20px;
      //   display: flex;
      //   flex-wrap: wrap;
      //   margin-top: 20px;
      //   animation: IconFadeIn 1s;
      //   .gnav-icon{
      //       margin-right: 20px;
      //   }
      //   .gnav-btn{
      //       width: 60%;
      //       color: #FFF!important;
      //       margin-top: 30px;
      //       margin-left: 0;
      //   }
      // }

    //   .sidebar-box {
    //     display: none;

    //     .logo_side {
    //       margin: 10px;
    //       animation: IconFadeIn 0.5s;
    //     }
    //   }
    // }
  }

  html.scroll-locked {
    overflow: hidden;

    // .hamburger-box {
    //   width: 60px;
    //   height: 60px;
    //   position: absolute;
    //   right: 5px;

    //   .gnav_bg {
    //     border-radius: 30px!important;
    //   }
    // }

    // .gnav_container {
    //   &.gnav_sp {
    //     .sidebar-box {
    //       display: block;
    //       position: fixed;
    //       width: calc(100% - 90px);
    //       height: 100%;
    //       animation: SidebarSlideIn 1s;
    //       overflow: scroll;
    //       -ms-overflow-style: none;
    //       scrollbar-width: none;
    //       &::-webkit-scrollbar{
    //         display: none;
    //       }
    //     }
    //   }
    // }
  }

  // ハンバーガーメニューのデザイン
  .hamburger {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    flex: 0 0 40px;
    font-size: 0;
    cursor: pointer;
    position: absolute;
    top: 0px;
    right: 0px;
    width: 60px;
    height: 60px;
    padding: 18px;

    &_top,
    &_btm {
      content: "";
    }

    &_top,
    &_mid,
    &_btm {
      display: inline-block;
      height: 3px;
      width: 100%;
      background-color: #001350;
      transition: opacity 0.1s, transform 0.3s;
    }

    &_mid {
      margin: 6px 0;
    }
  }

  // ハンバーガーメニュークリック時のデザイン
  #drawer-checkbox {
    &:checked ~ .hamburger {
      .hamburger {
        &_top,
        &_btm {
          width: 50%;
          position: absolute;
          top: 50%;
          left: 50%;
        }

        &_top {
          transform: translate(-50%, -50%) rotate(225deg);
        }

        &_mid {
          opacity: 0;
        }

        &_btm {
          transform: translate(-50%, -50%) rotate(-225deg);
        }
      }
    }

    &:checked ~ .drawer-close {
      display: block;
    }

    &:checked ~ .gnav_container.gnav_sp {
      display: block;
    }
    &:checked ~ .logo_side {
      display: none;
    }
  }

  .gnav_sp {
    // .gnav_items li {
      .dropdownSubMenu {
        width: 100%;
        position: relative;
        padding: 0;
        display: none;

        li a {
          margin-left: 15px;
          margin-right: -15px;
          margin-bottom: 10px;
          display: block;
          text-decoration: none;
        }
        .gnav-submenu {
          width: 100%;
        }
      }

      .dropdownSubMenu.open {
        display: block;
      }

      .open-icon {
        width: 41px;
        height: 41px;
        position: absolute;
        top: 0;
        right: 0;
        z-index: 10;
        cursor: pointer;

        &::after {
          content: "\e5cc";
          display: inline-block;
          font-family: Material icons;
          font-size: 20px;
          letter-spacing: normal;
          line-height: 1;
          flex: 0 0 auto;
          font-feature-settings: "liga" 1;
          top: 11px;
          position: absolute;
        }

        &.active {
          &::after {
            -webkit-transform: rotate(90deg);
            -moz-transform: rotate(90deg);
            -ms-transform: rotate(90deg);
            -o-transform: rotate(90deg);
            transform: rotate(90deg);
          }
        }
      }
    }
  }
}

// .gnav_draewr {
//   height: 100%;
//   width: 100%;

//   .section_inner {
//     display: flex;
//     align-items: center;
//     justify-content: space-between;
//     flex-wrap: wrap;
//     height: 100%;
//     width: 100%;
//     padding: 0 .5rem;
//     position: relative;

//     .gnav_bg {
//       height: 100%;
//       width: 100%;
//       position: absolute;
//       top: 0;
//       left: 0;
//       z-index: -1;
//     }
//   }

//   .logo_side {
//     height: 60px;
//     flex: 1 0 0;
//     padding: .5rem 0;

//     .header_logo {
//       width: 100%;
//       height: 100%;

//       span {
//         display: flex;
//         align-items: center;
//         height: 100%;
//       }
//     }

//     img {
//       height: 100%;
//       width: auto;

//       @supports (object-fit: contain) {
//         object-fit: contain;
//         object-position: 0 50%;
//       }
//     }
//   }

//   .gnav_container {
//     display: none;
//     width: 100%;

//     &.gnav_pc {
//       display: none;
//     }

    .gnav_items {
      li {
        opacity: 0;
        transform: translateX(2rem);
        @keyframes slide_in {
          0% {
            display: none;
          }
          1% {
            display: block;
            height: 1px;
          }
          99% {
            height: 100%;
          }
        }

        @mixin animationValue($name, $duration, $function, $delay, $state) {
          animation: $name $duration + s $function $delay + s $state;
        }

        @for $cnt from 1 through 20 {
          &:nth-child(#{$cnt}) {
            @include animationValue(
              slide_in,
              0.3,
              cubic-bezier(0.55, 0.055, 0.675, 0.19),
              $cnt * 0.1,
              forwards
            );
          }
        }

        @keyframes slide_in {
          100% {
            opacity: 1;
            transform: translateX(0);
          }
        }
      }

      a {
        display: flex;
        align-items: center;
        width: 100%;
        padding: 0.8rem 1.5rem 0.8rem 2rem;
      }
    }
  }
}

// PC用CSS
@media #{$pc_style_min} {
//   section:first-of-type .content{
//     padding: 25px;

//     [class^="mainvisual"] {
//       height: calc(100vh - 50px);
//     }
//   }

  // .gnav_standard_icon.gnav_draewr {
    // padding: 25px;

    .section_inner {
      height: 70px !important;
      padding: 0 !important;
    }

    .logo_side {
      height: 100%;
      flex: 0 0 auto;
      margin: 0 32px;
      padding: 1rem 0 !important;

      img {
        max-width: 200px;
        max-height: 60px;
      }
    }

    // .drawer_btn {
    //   display: none;
    // }

    .gnav_container {
      height: 100%;
      flex: 1 0 0%;

      .gnav_items {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        height: 100%;
      }

      .gnav_items li {
          height: 100%;
          border-top: 0;
          opacity: 1;
          transform: none;
          animation: none !important;
          padding: 0 12px;
          position: relative;
          // SubメニューStyle
          &:hover .dropdownSubMenu {
            border-top: 1px solid;
          }
          .dropdownSubMenu {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            margin: auto;
            padding: 0;

            li {
              overflow: hidden;
              height: 0;
              transition: 0.2s;
              margin-left: 0;
              white-space: nowrap;
            }

            li a {
              padding: 5px;
              margin-left: -5px;
              margin-right: -5px;
              margin-bottom: -5px;
              display: block;
              text-decoration: none;
            }
          }

          &:hover ul li {
            overflow: visible;
            height: 38px;
          }

        a {
          display: flex;
          align-items: center;
          justify-content: center;
          height: 100%;
          width: 100%;
          padding: 1.5rem 0.5rem;

          &:hover {
            text-decoration: underline;
          }
          &:after {
            content: none;
          }
        }
      }
    }
  }
}
</style>
