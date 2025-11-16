<template>
    <div class="home-page">
        <div class="content-wrapper">
            <span class="title">
                Navy Fund株式会社
            </span>
        </div>
        <div class="content-wrapper banner-wrapper">
            <img class="banner" src="../../assets/imgs/banner2.jpg" alt="">
        </div>
        <div class="content-page">
            <div class="content-wrapper">
                <strong class="title2">
                    Navy Fund株式会社について
                </strong>
                <span class="text">私たちの目標は、市場に垂直統合を提供するグループを創設することです。
                    これには、半導体ウェーハ工場や設計センターへの投資、製品設計、
                    生産プロセスと技術の移転、機器とアセンブリの供給、技術サービスの提供が含まれます。
                    さらなる改善やお客様とのより良い連携方法についてのご提案をお待ちしております。
                    このページでは、当社が完了したいくつかの主要プロジェクトと当社のビジネスパートナーに関する情報をご覧いただけます。
                </span>
                <div class="img-hover-wrapper">
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus1.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">关于半导体</div>
                                我们向您介绍电子、半导体、电信、材料和建筑行业。
                            </div>
                        </div>
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus2.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">公司介绍</div>
                                我们主要在日本和美国活跃业务。
                            </div>
                        </div>
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus3.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">业务介绍</div>
                                股票持有/投资、电子和半导体、新型建筑和涂料材料
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="divider">
                <hr>
            </div>
            <div class="content-wrapper">
                <strong class="title2">
                    入选理由
                </strong>
                <div class="img-hover-wrapper">
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/reason1.png" alt="" />
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/reason2.png" alt="" />
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/reason3.png" alt="" />
                    </div>
                </div>
            </div>
            <div class="divider">
                <hr>
            </div>
            <div class="content-wrapper">
                <strong class="title2">
                    新信息
                </strong>
                <div class="news-table">
                    <!-- 第一行 -->
                    <div class="news-row">
                        <div class="news-cell type">NEW</div>
                        <div class="news-cell date">2024-07-09</div>
                        <div class="news-cell content"></div>
                    </div>

                    <!-- 第二行 -->
                    <div class="news-row">
                        <div class="news-cell type">NEW</div>
                        <div class="news-cell date">2024-03-22</div>
                        <div class="news-cell content">代理运营*(东京都-山梨县)15-20%+清扫费</div>
                    </div>

                    <!-- 第三行 -->
                    <div class="news-row">
                        <div class="news-cell type">NEW</div>
                        <div class="news-cell date">2023-03-31</div>
                        <div class="news-cell content">NEWS</div>
                    </div>
                    <div class="more-info">
                        点击此处查看公告列表
                        <ChevronRight size="18" color="#fff" />
                    </div>
                </div>
            </div>
            <div class="divider">
                <hr>
            </div>
            <div class="content-wrapper">
                <strong class="title2">
                    商业合作伙伴
                </strong>
                <div class="img-hover-wrapper">
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus1.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">关于半导体</div>
                                我们向您介绍电子、半导体、电信、材料和建筑行业。
                            </div>
                        </div>
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus2.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">公司介绍</div>
                                我们主要在日本和美国活跃业务。
                            </div>
                        </div>
                    </div>
                    <div class="image-hover-box">
                        <img class="img" src="../../assets/imgs/aboutus3.jpg" alt="" />

                        <!-- 悬浮时显示的遮罩层 -->
                        <div class="mask">
                            <div class="mask-content">
                                <div class="mask-title">业务介绍</div>
                                股票持有/投资、电子和半导体、新型建筑和涂料材料
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ChevronRight } from 'lucide-vue-next';
</script>

<style scoped>
.img-hover-wrapper {
    display: flex;
    width: 100%;
    justify-content: space-around;
}

.image-hover-box {
    margin: 17px;
    position: relative;
    width: 200px;
    /* 可修改 */
    height: 200px;
    /* 可修改 */
    overflow: hidden;
}

/* 图片 */
.img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

/* 遮罩层（默认隐藏） */
.mask {
    position: absolute;
    left: 0;
    top: 0;
    width: 200px;
    height: 200px;
    background: rgba(44, 44, 44, 0.85);
    /* 半透明灰黑色遮罩 */
    color: #fff;
    opacity: 0;
    transition: 0.25s ease;
    display: flex;
    padding: 10px;
}

/* 文本内容可滚动 */
.mask-content {
    display: flex;
    flex-direction: column;
    overflow-y: auto;
    height: 100%;
    font-size: 12px;
    line-height: 24px;
    padding: 0 27px;
    align-items: center;
    color: #BBBBBB;
    text-align: center;
}

.mask-content .mask-title {
    color: white;
}

/* 悬停时显示遮罩 */
.image-hover-box:hover .mask {
    opacity: 1;
}

.home-page {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.divider {
    width: 100%;
    padding: 17px 0;
}

.divider hr {
    border-width: 0;
    margin: 32px 0;
    color: rgba(31, 31, 31, .15);
    background-color: rgba(31, 31, 31, .15);
    height: 1px;
}

.content-page {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 0 32px;
    max-width: 1020px;

}

.home-page>div {
    width: 100%;
}

.content-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
}

.title {
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 9px;
}

.banner-wrapper {
    position: relative;
}

.banner-wrapper::before {
    content: "";
    position: absolute;
    inset: 0;
    height: 150px;
    /* 渐变区域高度，可调 */
    pointer-events: none;
    background: linear-gradient(to bottom,
            #ffffff 0%,
            /* 顶部纯白 */
            rgba(255, 255, 255, 0.85) 30%,
            /* 深一点，接近白 */
            rgba(255, 255, 255, 0.55) 65%,
            /* 中间显著过渡 */
            rgba(255, 255, 255, 0) 100%
            /* 底部完全透明，与图片平滑融合 */
        );
    z-index: 2;
}

.banner {
    width: 100%;
}

.title2 {
    font-size: 42px;
    margin-top: 42px;
    margin-bottom: 21px;
}

.text {
    font-size: 32px;
    padding: 25px 0;
}

.news-table {
    display: flex;
    flex-direction: column;
    gap: 24px;
    /* 每行间距 */
    width: 100%;
}

.news-table .news-row {
    display: grid;
    grid-template-columns: 80px 120px 1fr;
    /* 三列：类型/日期/内容 */
    align-items: center;
    min-height: 30px;
    /* 每行最小高度，可根据需要调整 */
    gap: 16px;
}

.news-table .news-cell {
    padding: 4px 8px;
    white-space: normal;
    /* 自动换行 */
    overflow-wrap: break-word;
}

.news-table .type {
    font-weight: bold;
    background-color: #000;
    /* 黑色背景 */
    color: #fff;
    /* 白色文字 */
    text-align: center;
    /* 可选：文字居中 */
    padding: 2px 6px;
    /* 内边距 */
}

.news-table .date {
    color: #666;
}

.news-table .content {}

.news-table .more-info {
    display: flex;
    align-items: center;
    background-color: #000;
    color: #fff;
    padding: 6px 12px;
    margin-left: auto;
    font-size: 14px;
}
</style>