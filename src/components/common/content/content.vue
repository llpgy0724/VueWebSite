<template>
  <section class="div_content">
    <ul class="ul-header border-1px">

      <div class="left-menu" v-show="getGlobalInfo.isHigher768">
        <router-link to="/home">
          <li>首页</li>
        </router-link>
        <router-link to="/pic">
          <li>状态</li>
        </router-link>
        <router-link to="/music">
          <li>音乐</li>
        </router-link>
        <a href="http://www.panghu77.top" target="_black">
          <li>博客</li>
        </a>
        <router-link to="/about">
          <li>关于</li>
        </router-link>
      </div>

      <transitio name="fade">
        <div class="fixed-fade-menu" v-show="showLeftMenu" @click="hideLeftContent">
          <div class="fixed-menu-content" @click="hideLeftContent">
            <router-link to="/home">
              <li>首页</li>
            </router-link>
            <router-link to="/pic">
              <li>状态</li>
            </router-link>
            <router-link to="/music">
              <li>音乐</li>
            </router-link>
            <a href="http://www.panghu77.top" target="_black">
              <li>博客</li>
            </a>
            <router-link to="/about">
              <li>关于</li>
            </router-link>
          </div>
        </div>
      </transitio>
      <div class="right-menu">
        <span class="place" v-show="getPlace.region" :data-place="getPlace.region" @mouseover="showWeatherInfo" @mouseleave="hideWeatherInfo">
          {{getPlace.city}}
          <weather :isShow="showWeatherList"></weather>
        </span>
      </div>
    </ul>
  </section>
</template>

<script>
  
</script>

<style lang="scss" scoped>
  
</style>