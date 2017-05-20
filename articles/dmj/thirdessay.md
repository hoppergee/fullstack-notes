# 如何利用bootstrap 对图片进行排版（高级篇）

### 一  如何插入一张文字和文字背景图片藏在原图片下面的炫酷图片？


1. 效果图片：

   ![](https://ws3.sinaimg.cn/large/006tNbRwgy1ffrm2jpus5g30d00d175f.gif)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome7s.scss">
   </head>
   <body>
       <div class="persona-grid">
           <div class="container ">
               <div class="col-sm-4">
                   <div class="g10 persona-kira">
                       <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                           <div class="info-peek">
                               <div class="info-default active">
                                   <h2>Kira</h2>
                                       <p>Hopeful yogi, living the change she wants to see in the world</p>
                               </div>
                           </div>
                           <div class="overlay"></div>
                           <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                   </div>
               </div>
           </div>
       </div>
   </body>
   ```

   ```css
    .persona-grid {
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
   .persona-grid .persona-link .overlay {
       opacity: 0;
       position: absolute;
       top: 0;
       right: 0;
       bottom: 0;
       left: 0;
       z-index: 3
   }
   .persona-grid .persona-link:hover .info-peek .info-default,.persona-grid .persona-link:hover .overlay {
       opacity: 1
   }
   .persona-grid .persona-link>img {
       border: 1px solid #000;
   }
   .persona-kira .persona-link .overlay {
       background-color: rgba(143,150,203,0.85)
   }
   .persona-kira .persona-link img {
       border-color:  #8f96cb !important
   }

   ```

   ​

### 二 如何插入三张文字和文字背景图片藏在原图片下面的炫酷图片？


1. 效果图片：

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrm2lnrrtg30yd0d17a6.gif)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome7s.scss">
   </head>
   <body>
       <div class="persona-grid">
           <div class="container row-container">
               <div class="row">
                   <div class="col-sm-4">
                       <div class="g10 persona-kira">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
                   <div class="col-sm-4">
                       <div class="g10 persona-kira">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
                   <div class="col-sm-4">
                       <div class="g10 persona-kira">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
           </div>
       </div>
   </body>
   ```




### 三 如何插入三张不同文字和文字背景图片藏在原图片下面的炫酷图片？



1. 效果图片：

   ![](https://ws2.sinaimg.cn/large/006tNbRwgy1ffrm2njvbfg30yd0d144v.gif)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome7s.scss">
   </head>
   <body>
       <div class="persona-grid">
           <div class="container row-container">
               <div class="row">
                   <div class="col-sm-4">
                       <div class="g10 persona-kira">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
                   <div class="col-sm-4">
                       <div class="g10 persona-andrew">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/andrew/andrew_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/andrew/andrew_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
                   <div class="col-sm-4">
                       <div class="g10 persona-brett">
                           <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/brett/brett_face_m.jpg">
                               <div class="info-peek">
                                   <div class="info-default active">
                                       <h2>Kira</h2>
                                           <p>Hopeful yogi, living the change she wants to see in the world</p>
                                   </div>
                               </div>
                               <div class="overlay"></div>
                               <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/brett/brett_face_m.jpg" alt="Lights"  style="width:100%">
                           </a>
                       </div>
                   </div>
           </div>
       </div>
   </body>
   ```

   ```css
   +
   //*1.kira//
   .persona-grid .persona-link>img {
       border: 1px solid #000;
   }
   .persona-kira .persona-link .overlay {
       background-color: rgba(143,150,203,0.85)
   }
   .persona-kira .persona-link img {
       border-color:  #8f96cb !important
   }

   +
   //*2.andrew//
   .persona-andrew .persona-link .overlay {
      background-color:  rgba(116,174,122,0.85)

   }
   .persona-andrew .persona-link img {
      border-color:  #74ae7a !important
   }

   +
   //*3.brett//
   .persona-brett .persona-link .overlay {
      background-color:   rgba(221,154,73,0.85)

   }
   .persona-brett .persona-link img {
      border-color:  #dd9a49 !important
   }
   ```

   ​


### 四 作业 如何插入九张文字和文字背景图片藏在原图片下面的炫酷图片？


1. 效果图片：

   动态&静态效果图

   ![](https://ws3.sinaimg.cn/large/006tNbRwgy1ffrm2jpus5g30d00d175f.gif)

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrm2pwlh8j30zk0zb7gq.jpg)




2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome7s.scss">
   </head>
   <body>
     <div class="persona-grid">
         <div class="container row-container">
             <div class="row">
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
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
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
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
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
                 <div class="col-sm-4">
                     <div class="g10 persona-kira">
                         <a class="persona-link" href="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg">
                             <div class="info-peek">
                                 <div class="info-default active">
                                     <h2>Kira</h2>
                                         <p>Hopeful yogi, living the change she wants to see in the world</p>
                                 </div>
                             </div>
                             <div class="overlay"></div>
                             <img class="img-rounded" src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" alt="Lights"  style="width:100%">
                         </a>
                     </div>
                 </div>
         </div>
     </div>
   </body>
   ```

   ​


### 五 作业 如何插入九张不同文字和文字背景图片藏在原图片下面的炫酷图片？

1. 效果图片：

   动态&静态效果图

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrm4wyf6ng30b50ajac6.gif)

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrm4v8vjbj30zk0w1b29.jpg)

   ​

   ​

2. 如何做？

   ```html
   <head>
      <link rel="stylesheets" type="text/scss" href="welcome9s.scss">
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

   ```css
    .persona-grid {
       margin-top: 20px;
       margin-bottom: 20px;
    }
    //* 调整图片位置使用！＊//

    @media (min-width: 480px) {
       .persona-grid .row {
        display:flex;
       }
    }
    //* 调整图片大小使用，如果没有这个css，背景图片会变得很大，且两张图片不会并列排列！＊//

    .persona-grid .persona-link {
       display: block;
       position: relative;
    }
    //* 调整链接位置，如果没有这个css，鼠标移动到图片时，链接的阴影部分会占据整个屏幕 *//

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
    //* 调整字体的位置，z-index: 4 & position: absolute使字体可以悬浮于北京图片调整链接位置 *//

    .persona-grid .persona-link .info-default {
       opacity: 0;
       display: block;
       position: absolute;
       width: 100%
    }
    //* 作用是使得白色自字体藏在图片下面，只有鼠标移动到图片上时，字体才会和背景图片一起出现 *//
   ```


    .persona-grid .persona-link .overlay {
       opacity: 0;
       position: absolute;
       top: 0;
       right: 0;
       bottom: 0;
       left: 0;
       z-index: 3
    }
    //* 调整背景蓝色图片使用，如果没有这个css，鼠标移动到图片时，背景的蓝色图片将不会出现 和使得蓝色背景图片在实际图片下面。 *//

    .persona-grid .persona-link>img {
       border: 1px solid #000;
    }
    //* 调整图片边框使用，如果没有这个css，图片将不会显示边框 *//


    .persona-grid .persona-link:hover .info-peek .info-default,.persona-grid .persona-link:hover .overlay {
       opacity: 1
    }
    //* 当鼠标移动到图片时，可以出现蓝色背景和字体 *//


   //*1.amy
    .persona-amy .persona-link .overlay {
       background-color: rgba(35,165,189,0.85)

    }
    //* 给amy这个人的图片上加入一张蓝色背景的图片 *//

    .persona-amy .persona-link img {
       border-color: #23a5bd !important
    }
    //* 给amy这个人的图片上加上蓝色边框 *//


   //*2.ida
   .persona-ida .persona-link .overlay {
       background-color:  rgba(91,63,130,0.85)
   }
    .persona-ida .persona-link img {
       border-color: #5b3f82 !important
    }

    //*3. matt
    .persona-matt .persona-link .overlay {
       background-color:   rgba(202,65,66,0.85)

    }
    .persona-matt .persona-link img {
       border-color: #ca4142 !important
    }

    //*4.jandd
    .persona-jandd .persona-link .overlay {
       background-color:   rgba(158,127,87,0.85)

    }
    .persona-jandd .persona-link img {
       border-color:  #9e7f57 !important
    }


    //*5.brett
    .persona-brett .persona-link .overlay {
       background-color:   rgba(221,154,73,0.85)

    }
    .persona-brett .persona-link img {
       border-color:  #dd9a49 !important
    }


    //*6.kira
    .persona-kira .persona-link .overlay {
       background-color:  rgba(143,150,203,0.85)

    }
    .persona-ikira .persona-link img {
       border-color:  #8f96cb !important
    }


    //*7.andrew
    .persona-andrew .persona-link .overlay {
       background-color:  rgba(116,174,122,0.85)

    }
    .persona-andrew .persona-link img {
       border-color:  #74ae7a !important
    }


    //*8.linda
    .persona-linda .persona-link .overlay {
       background-color:  rgba(197,61,139,0.85)

    }
    .persona-linda .persona-link img {
       border-color:  #c53d8b !important
    }


    //*9.sarah
    .persona-sarah .persona-link .overlay {
       background-color:  rgba(108,100,116,0.85)

    }
    .persona-sarah .persona-link img {
       border-color:  #6c6474 !important
    }





### 六 温馨提示 & 资源分享

1. 如果你看不懂，你可能需要以下背景知识：

* [如何利用bootstrap 对图片进行排版（进阶篇）]()

- [如何利用bootstrap 对图片进行排版（基础篇）]()


- [Bootstrap Images](https://www.w3schools.com/bootstrap/bootstrap_images.asp)

- [Bootstrap Grids](https://www.w3schools.com/bootstrap/bootstrap_grid_basic.asp)

  ​


2. 如果你对董明娟童鞋是如何写出用bootstrap对图片进行排版的小教程感兴趣,推荐看以下文章：

* [复盘总结－－花了28+6小时做出含炫酷图片的页面 & 写出分享的系列教程]()

   ​

   ​
