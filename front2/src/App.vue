<template>
  <a-layout id="components-layout-demo-top" class="layout">
    <a-layout-header>
      <div class="logo" />
      <a-menu
        theme="dark"
        mode="horizontal"
        :defaultSelectedKeys="['2']"
        :style="{ lineHeight: '64px' }"
      >
        <a-menu-item key="1">DatsPush</a-menu-item>
        <a-menu-item key="2">MediaVenus</a-menu-item>
        <a-menu-item key="3">LostPlanet</a-menu-item>
      </a-menu>
    </a-layout-header>
    <a-layout-content style="padding: 0 50px">
      <router-view />
    </a-layout-content>
    <a-layout-footer style="text-align: center">
      MakeYourWay © 2019 Created by Balkhaev
    </a-layout-footer>
  </a-layout>
</template>
<style>
  body {
    background-color: #f0f2f5 !important;
  }
  #components-layout-demo-top .logo {
    width: 120px;
    height: 31px;
    background: rgba(255,255,255,.2);
    margin: 16px 24px 16px 0;
    float: left;
  }
</style>
