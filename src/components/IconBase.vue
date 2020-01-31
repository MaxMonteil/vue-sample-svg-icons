<template functional>
  <svg xmlns="http://www.w3.org/2000/svg"
    :width="props.size"
    :height="props.size"
    viewBox="0 0 18 18"
    :aria-labelledby="props.iconName"
    role="presentation"
    :class="[
      data.class,
      data.staticClass
    ]"
    :style="[
      data.style,
      data.staticStyle
    ]"
  >
    <title :id="props.iconName" lang="en">{{ props.iconName.replace(/-/g, ' ') }} icon</title>
    <g :fill="props.iconColor">
      <component :is="injections.components[props.iconName]" />
    </g>
  </svg>
</template>

<script>
export default {
  inject: {
    components: {
      default: {
        // Add new icons here using kebab-case keys:
        // 'icon-name': () => import('./icons/IconFullMoon'),
        'box': () => import('./icons/IconBox'),
        'calendar': () => import('./icons/IconCalendar'),
        'envelope': () => import('./icons/IconEnvelope'),
        'garbage': () => import('./icons/IconGarbage'),
        'image': () => import('./icons/IconImage'),
        'moon': () => import('./icons/IconMoon'),
        'write': () => import('./icons/IconWrite')
      }
    }
  },
  props: {
    iconName: {
      type: String,
      default: 'box'
    },
    size: {
      type: [Number, String],
      default: 18
    },
    iconColor: {
      type: String,
      default: 'currentColor'
    }
  }
}
</script>

<style scoped>
svg {
  display: inline-block;
  vertical-align: baseline;
  margin-bottom: -2px; /* yes, I'm that particular about formatting */
}
</style>
