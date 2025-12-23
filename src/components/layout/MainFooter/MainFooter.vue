<template>
  <footer class="main-footer d-flex p-2 px-3 bg-white border-top">
    
  </footer>
</template>

<script>
const defaultMenuItems = [{
  title: 'Home',
  to: 'https://git.orangeca.ir/A.Namazi/recommendation-dashboard/',
}, {
  title: 'GitHub',
  to: 'https://git.orangeca.ir/A.Namazi/recommendation-dashboard',
}, {
  title: 'Document',
  to: 'https://git.orangeca.ir/A.Namazi/recommendation-dashboard',
}, {
  title: 'API',
  to: '/apidocs/',
}];

export default {
  name: 'main-footer',
  props: {
    /**
       * The footer menu items.
       */
    menuItems: {
      type: Array,
      default() {
        return defaultMenuItems;
      },
    },
    /**
       * The copyright information.
       */
    copyright: {
      type: String,
      default: `Copyright © ${new Date().getFullYear()} zhenghaoz`,
    },
    /**
       * Whether the footer should be wrapped in a container, or not.
       */
    contained: {
      type: Boolean,
      default: false,
    },
  },
};
</script>
