<template>
  <div class="layout-container">

    <!-- 顶部导航栏 -->
    <header class="header">
      <div class="logo-box fade-in delay-1">
        <img src="../assets/imgs/logo2.png" alt="">
      </div>

      <div class="nav-box fade-in delay-2">
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

    <footer class="footer">
      <div class="footer-container">
        <div class="footer-left">
          <img src="../assets/imgs/logo-white.png" alt="Logo" class="footer-logo" />
          <div class="phone left-item">
            <Phone size="18" color="#fff" /> : 03-5577-4248
          </div>
          <div class="left-item">
            <Mail size="18" color="#fff" /> : lawmoo@navyfundtokyo.com
          </div>
        </div>

        <!-- 右边导航栏目 -->
        <div class="footer-right">
          <ul class="footer-list">
            <li class="footer-link">
              トップ
            </li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link">
              本社概要
            </li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link">
              投資部
            </li>
            <li class="footer-link">
              株式持株保有/投資
            </li>
            <li class="footer-link">
              会社売買
            </li>
            <li class="footer-link">
              コンサルタント
            </li>
            <li class="footer-link">
              半導体
            </li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link">
              半導体投資
            </li>
            <li class="footer-link">
              半導体投資
            </li>
          </ul>
        </div>
      </div>
      <div class="copyright">
        Copyright © Navy Fund株式会社. All Rights Reserved.
      </div>
    </footer>

  </div>
</template>

<script setup>
import { Phone, Mail } from 'lucide-vue-next';
</script>

<style scoped>
.left-item{
  display: flex;
  align-items: center;
  gap: 8px;
}

.phone {

}

.footer {
  background-color: #000;
  color: #ffffff66;
  /* 底部背景色 */
  padding: 70px 150px 45px;
}

.footer-container {
  display: flex;
  /* 左右分布 */
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  /* 响应式换行 */
  border-bottom: 1px solid rgba(255, 255, 255, 0.05);
}

.footer-left {
  display: flex;
  flex-direction: column;
  gap: 15px;
  color: #fff;
}

.footer-logo {
  width: 300px;
  object-fit: contain;
  margin-right: 10px;
}

.footer-text {
  font-size: 18px;
  font-weight: bold;
}

.footer-right {
  width: 45%;
  display: grid;
  grid-template-columns: repeat(3, 1fr) auto;
  grid-gap: 80px;
}

.footer-list {
  display: flex;
  flex-direction: column;
}

.footer-list .footer-link:first-child {
  color: #fff;
  font-size: 16px;
  margin-bottom: 30px;
  /* 示例样式 */
}

.footer-link {
  text-decoration: none;
  transition: color 0.3s;
  cursor: pointer;
  font-size: 14px;
  margin-bottom: 15px;
}

.footer-link:hover {
  color: #fff;
  /* 悬停颜色 */
}

.copyright {
  padding-top: 35px;
  color: #fff;

}

/* 响应式处理：屏幕小于 600px 时换行 */
@media (max-width: 600px) {
  .footer-container {
    flex-direction: column;
    align-items: flex-start;
    gap: 10px;
  }

  .footer-right {
    gap: 10px;
  }
}

/* 淡入基础动画 */
.fade-in {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeInUp 0.8s ease-out forwards;
}

/* 延迟控制，让元素依次出现 */
.delay-1 {
  animation-delay: 0.1s;
}

.delay-2 {
  animation-delay: 0.3s;
}

.delay-3 {
  animation-delay: 0.5s;
}

@keyframes fadeInUp {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

/* 顶部导航栏整体 */
.header {
  width: 100%;
  height: 140px;
  /* 包含上下 padding */
  padding: 20px;
  /* 上下左右20px */
  display: flex;
  align-items: center;
  justify-content: center;
  background: #fff;
}

/* 左边 logo 区域（模拟图片用 div） */
.logo-box {
  height: 86px;
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