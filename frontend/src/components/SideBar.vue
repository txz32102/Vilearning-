<template>
    <SidebarMenu :menu="menu" theme="white-theme" :width="'200px'"/>
  </template>
  
  <script>
  import {SidebarMenu} from 'vue-sidebar-menu'
  import 'vue-sidebar-menu/dist/vue-sidebar-menu.css'
  import '@fortawesome/fontawesome-free/css/all.css'
  import llt from '@/assets/icons/llt.png';
  import ht from '@/assets/icons/ht.png';
  import cs from '@/assets/icons/cs.png';
  import ls from '@/assets/icons/ls.png';
  import xh from '@/assets/icons/xh-optimize.gif';
  export default {
    name: "SideBar",
    components: {
      SidebarMenu,
    },
    data() {
        return {
          menu: [
            {
              header: 'ViLearning',
              hiddenOnCollapse: true,
            },
            {
              href: '/table',
              title: 'table',
              icon: {
                element: 'img',
                attributes: { src: cs },
            },
            },
            {
              href: '/Debug',
              title: 'Debug',
              icon: {
                element: 'img',
                attributes: { src: ht },
            },
            },
            {
              href: '/Result',
              title: 'Result',
              icon: {
                element: 'img',
                attributes: { src: ls },
            },
            },
            {
              href: '/Contact',
              title: 'Contact',
              icon: {
                element: 'img',
                attributes: { src: llt },
            },
            },
            {
              href: '/FAQ',
              title: 'FAQ',
              icon: {
                element: 'img',
                attributes: { src: xh },
            },
            }
          ],
        }
      },
  }
  </script>
  
  <style scoped>
  </style>
  