<template>
  <transition name="back-to-top-fade">
    <div 
      class="vue-back-to-top" id="buttonbacktotop"
      pill
      :style="`bottom:${this.bottom};right:${this.right};`" 
      v-show="visible" 
      @click="backToTop">
      <slot>
        <div class="default">
          <b-icon icon="arrow90deg-up" class="top-arrow"></b-icon>
        </div>
      </slot>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'BackToTop',
  props: {
    text: {
      type: String,
      default: 'Voltar ao topo',
    },
    visibleoffset: {
      type: [String, Number],
      default: 600,
    },
    visibleoffsetbottom: {
      type: [String, Number],
      default: 0,
    },
    right: {
      type: String,
      default: '20px',
    },
    bottom: {
      type: String,
      default: '30px',
    },

  },
  data () {
    return {
      visible: false
    }
  },
  mounted () {
    window.smoothscroll = () => {
      let currentScroll = document.documentElement.scrollTop || document.body.scrollTop
      if (currentScroll > 0) {
        window.requestAnimationFrame(window.smoothscroll)
        window.scrollTo(0, Math.floor(currentScroll - (currentScroll / 5)))
      }
    }
    window.addEventListener('scroll', this.catchScroll)
  },
  destroyed () {
    window.removeEventListener('scroll', this.catchScroll)
  },
  methods: {
    /**
     * Catch window scroll event 
     * @return {void}
     */
    catchScroll () {
      const pastTopOffset = window.pageYOffset > parseInt(this.visibleoffset)
      const pastBottomOffset = window.innerHeight + window.pageYOffset >= document.body.offsetHeight - parseInt(this.visibleoffsetbottom)
      this.visible = parseInt(this.visibleoffsetbottom) > 0 ? pastTopOffset && !pastBottomOffset : pastTopOffset
      this.scrollFn(this)
    },
    /**
     * The function who make the magics
     * @return {void}
     */
    backToTop () {
      window.smoothscroll()
      this.$emit('scrolled')
    }
  },
}
</script>

<style lang="scss">
  .vue-back-to-top .default{
    background: #FF1744;
    font-family: 'Varela Round';
    font-size: 12px;
    color: #ffffff;
    width: 50px;
    border-radius: 6px;
  }
  .top-arrow {
    font-size: 23px;
    margin-top: 3px;
  }
</style>