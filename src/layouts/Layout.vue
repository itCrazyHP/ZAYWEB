<template>
    <div class="layout-container">
  
      <!-- 顶部导航栏 -->
      <header class="header">
        <!-- 左边“图标”盒子 -->
        <div class="logo-box">
            <img src="../assets/imgs/logo.jpg" alt="">
        </div>
  
        <!-- 右边导航 -->
        <div class="nav-box">
          <span class="nav-item">トップ</span>
          <span class="nav-item">本社概要</span>
          <span class="nav-item">投資部</span>
          <span class="nav-item">半導体投資</span>
        </div>
      </header>
  
      <!-- 主内容 -->
      <main class="main">
        <router-view />
      </main>
  
    </div>
  </template>
  
  <script>
  export default {
    name: "Layout",
  };
  </script>
  
  <style scoped>
  /* 顶部导航栏整体 */
  .header {
    width: 100%;
    height: 140px;              /* 包含上下 padding */
    padding: 20px;              /* 上下左右20px */
    display: flex;
    align-items: center;
    justify-content: center;
    background: #fff;
  }
  
  /* 左边 logo 区域（模拟图片用 div） */
  .logo-box {
    height: 86px;
    background: #ccc;
    display: flex;
    justify-content: center;
    position: absolute;
    left: 20px;
    align-items: center;
    font-weight: bold;
  }
  
  /* 右边导航栏 */
  .nav-box {
    flex: 1;                     
    display: flex;
    align-items: center;
    gap: 30px;     
    justify-content: center;              
  }
  
  .nav-item {
    font-size: 13px;
    cursor: pointer;
  }
  </style>
  