#  如何利用bootstrap 对图片进行排版（基础篇）

### 一  如何插入一张Rounded Corners的图片？


1. 效果图片：

   ![](https://ws1.sinaimg.cn/large/006tNbRwgy1ffrlhe0mahj30pa0iw7bq.jpg)




2. 如何做？

```html
<!DOCTYPE html>
<html>

      <head>
      </head>

    <body>
        <div class="container">
          <h2>Rounded Corners</h2>
          <p>The .img-rounded class adds rounded corners to an image </p>
          <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
        </div>
    </body>

</html>
```



###二 如何横排插入三张Rounded Corners的图片


1. 效果图片:

   ![](https://ws3.sinaimg.cn/large/006tNbRwgy1ffrlhgz3hij31kw0gbqcv.jpg)

   ​

2. 如何做？

```html
<!DOCTYPE html>
<html>
    <head>
    </head>

    <body>
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                  <div class="container">
                      <h2>Rounded Corners</h2>
                      <p> rounded corners to an image </p>
                      <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                  </div>
                </div>
                <div class="col-md-4">
                  <div class="container">
                      <h2>Rounded Corners</h2>
                      <p>rounded corners to an image </p>
                      <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                  </div>
                </div>
                <div class="col-md-4">
                  <div class="container">
                      <h2>Rounded Corners</h2>
                      <p>rounded corners to an image </p>
                      <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                  </div>
                </div>
            </div>
        </div>
    </body>
</html>

```




### 三  如何在一张页面中插入九张Rounded Corners 图片


1. 效果图片:

   ![](https://ws4.sinaimg.cn/large/006tNbRwgy1ffrlhjidlnj30zk10k142.jpg)

   ​

   ​

2. 如何做？

   ```html
   <!DOCTYPE html>
   <html>
       <head>
       </head>

       <body>
           <div class="container">
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p> rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p> rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p> rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
           </div>
       </body>
   </html>
   ```

   ​





### 四 作业：如何在一张页面中插入三张Rounded Corners &  三张Thumbnail & Circle 图片

1. 效果图片：

   ![](https://ws4.sinaimg.cn/large/006tNbRwgy1ffrlhlg8amj30zk0t8ain.jpg)

   ​

2. 如何做：

   ```html
   <!DOCTYPE html>
   <html>
       <head>
       </head>

       <body>
           <div class="container">
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p> rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Rounded Corners</h2>
                         <p>rounded corners to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Circle</h2>
                         <p> Circle to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-circle" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Circle</h2>
                         <p>Circle to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-circle" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Circle</h2>
                         <p>Circle to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-circle" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
               <div class="row">
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Thumbnail</h2>
                         <p> Thumbnail to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-thumbnail" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Thumbnail</h2>
                         <p>Thumbnail to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-thumbnail" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
                   <div class="col-md-4">
                     <div class="container">
                         <h2>Thumbnail</h2>
                         <p>Thumbnail to an image </p>
                         <img src="http://personaproject.martinprosperity.org/wp-content/themes/personaproject/images/personas/kira/kira_face_m.jpg" class="img-thumbnail" alt="Cinque Terre" width="304" height="236">
                     </div>
                   </div>
               </div>
           </div>
       </body>
   </html>

   ```

   ​

   ​


### 五 温馨提示 & 资源分享
1. 如果你看不懂，你可能需要以下背景知识：

- [Bootstrap Images](https://www.w3schools.com/bootstrap/bootstrap_images.asp)

- [Bootstrap Grids](https://www.w3schools.com/bootstrap/bootstrap_grid_basic.asp)

  ​


2. 如果你对董明娟童鞋是如何写出用bootstrap对图片进行排版的小教程感兴趣,推荐看以下文章：

* [如何利用bootstrap 对图片进行排版（进阶篇）]()


- [如何利用bootstrap 对图片进行排版（高级篇）]()

  ​


3. 如果你对董明娟童鞋是如何写出用bootstrap对图片进行排版的小教程感兴趣,推荐看以下文章：

* [复盘总结－－花了28+6小时做出含炫酷图片的页面 & 写出分享的系列教程]()
