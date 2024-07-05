<template>
  <div class="sidebar" :data="backgroundColor">
    <!--
            Tip 1: you can change the color of the sidebar's background using: data-background-color="white | black | darkblue"
            Tip 2: you can change the color of the active button using the data-active-color="primary | info | success | warning | danger"
        -->
    <!-- -->
    <div class="sidebar-wrapper" id="style-3">
      <div class="logo">
        <a
          href="https://fr.linkedin.com/in/amine-itji-5a8696268?challengeId=AQE_Dow0HS0K4wAAAZCFBab3VnLPnlKtReg-gq4xdQWCIiYpCsVn5tphS8ec1PTcmzSuc1tbgQqyMhANqX2ZMlr8-xWrbNB4jA&submissionId=0f9b6960-c171-df17-9643-66299ede0752&challengeSource=AgE_YRFAi8lLOQAAAZCFBbzn9lxHdSRBIFJv9uoWZvz3zjUn-duHdkZ8PHTlLPs&challegeType=AgENRcrA-wgnyQAAAZCFBbzqSblDA-WrtrTHm7ceKci0bJbpFHPg1SY&memberId=AgGs3QeZOEV-VQAAAZCFBbzuFfGfsWTtI9GheLmfHTMzXUU&recognizeDevice=AgG46hBNjhTXeAAAAZCFBbzyzoRj4YwLpMgH_mIcMPQqc7oufmOx"
          aria-label="sidebar mini logo"
          class="simple-text logo-mini"
        >
          <div class="logo-img" :class="{ 'logo-img-rtl': $rtl.isRTL }">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/LinkedIn_icon_circle.svg/640px-LinkedIn_icon_circle.svg.png"
              alt=""
            />
          </div>
        </a>
        <a href="https://fr.linkedin.com/in/amine-itji-5a8696268?challengeId=AQE_Dow0HS0K4wAAAZCFBab3VnLPnlKtReg-gq4xdQWCIiYpCsVn5tphS8ec1PTcmzSuc1tbgQqyMhANqX2ZMlr8-xWrbNB4jA&submissionId=0f9b6960-c171-df17-9643-66299ede0752&challengeSource=AgE_YRFAi8lLOQAAAZCFBbzn9lxHdSRBIFJv9uoWZvz3zjUn-duHdkZ8PHTlLPs&challegeType=AgENRcrA-wgnyQAAAZCFBbzqSblDA-WrtrTHm7ceKci0bJbpFHPg1SY&memberId=AgGs3QeZOEV-VQAAAZCFBbzuFfGfsWTtI9GheLmfHTMzXUU&recognizeDevice=AgG46hBNjhTXeAAAAZCFBbzyzoRj4YwLpMgH_mIcMPQqc7oufmOx" class="simple-text logo-normal">
          {{ title }}
        </a>
      </div>
      <slot> </slot>
      <ul class="nav">
        <!--By default vue-router adds an active class to each route link. This way the links are colored when clicked-->
        <slot name="links">
          <sidebar-link
            v-for="(link, index) in sidebarLinks"
            :key="index"
            :to="link.path"
            :name="link.name"
            :icon="link.icon"
          >
          </sidebar-link>
        </slot>
      </ul>
    </div>
  </div>
</template>
<script>
import SidebarLink from "./SidebarLink";

export default {
  props: {
    title: {
      type: String,
      default: "ITJI Amine",
    },
    backgroundColor: {
      type: String,
      default: "vue",
    },
    activeColor: {
      type: String,
      default: "success",
      validator: (value) => {
        let acceptedValues = [
          "primary",
          "info",
          "success",
          "warning",
          "danger",
        ];
        return acceptedValues.indexOf(value) !== -1;
      },
    },
    sidebarLinks: {
      type: Array,
      default: () => [],
    },
    autoClose: {
      type: Boolean,
      default: true,
    },
  },
  provide() {
    return {
      autoClose: this.autoClose,
      addLink: this.addLink,
      removeLink: this.removeLink,
    };
  },
  components: {
    SidebarLink,
  },
  computed: {
    /**
     * Styles to animate the arrow near the current active sidebar link
     * @returns {{transform: string}}
     */
    arrowMovePx() {
      return this.linkHeight * this.activeLinkIndex;
    },
    shortTitle() {
      return this.title
        .split(" ")
        .map((word) => word.charAt(0))
        .join("")
        .toUpperCase();
    },
  },
  data() {
    return {
      linkHeight: 65,
      activeLinkIndex: 0,
      windowWidth: 0,
      isWindows: false,
      hasAutoHeight: false,
      links: [],
    };
  },
  methods: {
    findActiveLink() {
      this.links.forEach((link, index) => {
        if (link.isActive()) {
          this.activeLinkIndex = index;
        }
      });
    },
    addLink(link) {
      const index = this.$slots.links.indexOf(link.$vnode);
      this.links.splice(index, 0, link);
    },
    removeLink(link) {
      const index = this.links.indexOf(link);
      if (index > -1) {
        this.links.splice(index, 1);
      }
    },
  },
  mounted() {
    this.$watch("$route", this.findActiveLink, {
      immediate: true,
    });
  },
};
</script>
