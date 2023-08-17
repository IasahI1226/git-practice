<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>9章演習</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header></header>
    <main>
      <div class="step-box">
        <div class="step-img1"></div>
        <span class="step-num">step1</span>
        <h3 class="title">タイトルが入ります</h3>
        <p class="text">
          文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。
        </p>
      </div>

      <div class="step-box">
        <div class="step-img2"></div>
        <span class="step-num">step2</span>
        <h3 class="title">タイトルが入ります</h3>
        <p class="text">
          文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。
        </p>
      </div>

      <div class="step-box">
        <div class="step-img3"></div>
        <span class="step-num">step3</span>
        <h3 class="title">タイトルが入ります</h3>
        <p class="text">
          文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。文章が入ります。
        </p>
      </div>
    </main>
    <footer></footer>
  </body>
</html>

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

header {
  height: 50px;
  background-color: #ff9a4b;
}

main {
  width: 960px;
  margin: 50px auto;
  display: flex;
}

.step-box {
  width: 300px;
  margin-right: 30px;
  padding: 10px;
  position: relative;
  background-color: #eee;
}

.step-box:last-child {
  margin-right: 0;
}

.step-img1 {
  height: 150px;
  background-image: url(img/flow01.png);
  background-position: bottom;
  background-size: cover;
}

.step-img2 {
  height: 150px;
  background-image: url(img/flow02.png);
  background-position: bottom;
  background-size: cover;
}

.step-img3 {
  height: 150px;
  background-image: url(img/flow03.png);
  background-position: bottom;
  background-size: cover;
}

.step-num {
  position: absolute;
  top: 0;
  left: 0;
  background-color: #ff9a4b;
  color: #fff;
}

.title {
  margin: 15px 0 5px;
}

footer {
  height: 50px;
  background-color: #aaa;
}

@media(max-width:768px){
  main{
    display: block;
    max-width: 100%;
  }
  header{
    height: 50px;
    max-width: 100%;
  }
  .step-box{
    width: 90%;
    margin: 0 5% 20px;

  }
}