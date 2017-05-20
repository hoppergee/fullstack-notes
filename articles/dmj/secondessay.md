# 如何利用bootstrap 对图片进行排版（进阶篇）

### 一  如何插入一张文字藏在图片下面的炫酷图片？


1. 效果图片：

   ![](https://ws2.sinaimg.cn/large/006tNbRwgy1ffrlpscbqfg30e40d1n1j.gif)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome8s.scss">
   </head>
   <body>
       <div class="persona-grid">
           <div class="container ">
               <div class="col-sm-4">
                   <div class="persona-kira">
                       <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                           <div class="info-peek">
                               <div class="info-default active">
                                   <h2>Kira</h2>
                                       <p>Hopeful yogi, living the change she wants to see in the world</p>
                               </div>
                           </div>
                           <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                   </div>
               </div>
           </div>
       </div>
   </body>
   ```

   ```CSS
   persona-grid {
      margin-top: 20px;
      margin-bottom: 20px;
   }
   //* 调整图片位置使用！＊//

   @media (min-width: 480px) {
       .persona-grid .row {
        display:flex;
       }
   }
   .persona-grid .persona-link {
       display: block;
       position: relative;
   }
   .persona-grid .persona-link .info-peek {
       text-align: center;
       position: absolute;
       top: 0;
       right: 0;
       bottom: 0;
       left: 0;
       z-index: 4;
       color: #fff
   }
   .persona-grid .persona-link .info-default {
       opacity: 0;
       display: block;
       position: absolute;
       width: 100%
   }
   .persona-grid .persona-link:hover .info-peek .info-default {
       opacity: 1
   }
   ```

   ​




### 二 如何插入三张文字藏在图片下面的炫酷图片？


1. 效果图片：

   ![](https://ws4.sinaimg.cn/large/006tNbRwgy1ffrlpz86oeg30xu0d1apr.gif)


2. 如何做？

   ```html
    <head>
      <link rel="stylesheets" type="text/scss" href="welcome8s.scss">
   </head>
   <body>
     <div class="persona-grid">
         <div class="container row-container">
             <div class="row">
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
         </div>
     </div>
   </body>
   ```

   ​


### 三 作业 如何插入9张文字藏在图片下面的炫酷图片？


1. 效果图片:

   动图 &静图![](https://ws2.sinaimg.cn/large/006tNbRwgy1ffrlpscbqfg30e40d1n1j.gif)

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrlq1mne5j30zk0zbwqy.jpg)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome8s.scss">
   </head>
   <body>
     <div class="persona-grid">
         <div class="container row-container">
             <div class="row">
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
         </div>
     </div>
     <div class="persona-grid">
         <div class="container row-container">
             <div class="row">
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
         </div>
     </div>
     <div class="persona-grid">
         <div class="container row-container">
             <div class="row">
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
         </div>
     </div>
   </body>
   ```

   ​


### 四 温馨提示 & 资源分享

1. 如果你看不懂，你可能需要以下背景知识：
* [如何利用bootstrap 对图片进行排版（基础篇）]()

- [Bootstrap Images](https://www.w3schools.com/bootstrap/bootstrap_images.asp)

- [Bootstrap Grids](https://www.w3schools.com/bootstrap/bootstrap_grid_basic.asp)

  ​

2. 如果你对董明娟童鞋是如何写出用bootstrap对图片进行排版的小教程感兴趣,推荐看以下文章：

- [如何利用bootstrap 对图片进行排版（高级篇）]()

  ​

3. 如果你对董明娟童鞋是如何写出用bootstrap对图片进行排版的小教程感兴趣,推荐看以下文章：

- [复盘总结－－花了28+6小时做出含炫酷图片的页面 & 写出分享的系列教程]()
