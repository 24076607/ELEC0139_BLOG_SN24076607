<template>
    <div class="article-container">
      <article-header
        title="你的文章标题"
        subtitle="文章副标题"
        author="你的名字"
      />
      
      <div class="article-content">
        <article-section id="section1" title="第一章节">
          <p>文章内容...</p>
          <img src="@/assets/images/diagram1.png" alt="示意图1">
          
          <!-- 交互组件示例 -->
          <demo1-component />
        </article-section>
        
        <article-section id="section2" title="第二章节">
          <p>更多内容...</p>
          
          <!-- 视频示例 -->
          <div class="video-container">
            <video controls>
              <source src="@/assets/videos/demo.mp4" type="video/mp4">
            </video>
          </div>
          
          <!-- 另一个交互组件 -->
          <demo2-component />
        </article-section>
        
        <!-- 更多章节 -->
      </div>
      
      <footer-component />
    </div>
  </template>
  
  <script setup>
  import ArticleHeader from './ArticleHeader.vue';
  import ArticleSection from './ArticleSection.vue';
  import FooterComponent from './Footer.vue';
  import Demo1Component from './interactive/Demo1.vue';
  import Demo2Component from './interactive/Demo2.vue';
  </script>
  
  <style scoped>
  .article-container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .video-container {
    width: 100%;
    margin: 20px 0;
  }
  
  .video-container video {
    width: 100%;
    height: auto;
  }
  </style>