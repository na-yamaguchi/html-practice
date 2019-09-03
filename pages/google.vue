<template>
  <div class="container">
    <div>
      <header>
        <ul class="header-menu">
          <li><a href="#">Gmail</a></li>
          <li><a href="#">画像</a></li>
          <li>
            <a href="#">
              <div class="appli-icon"></div>
            </a>
          </li>
          <li>
            <a href="#">
              <img src="@/pages/myicon.JPG" class="user-icon" />
            </a>
          </li>
        </ul>
      </header>
      <div class="main">
        <h1>
          <span class="blue">G</span>
          <span class="red">o</span>
          <span class="yellow">o</span>
          <span class="blue">g</span>
          <span class="green">l</span>
          <span class="red">e</span>
        </h1>
        <div class="search">
          <input type="text" class="search-box" />
          <input class="btn search-btn" value="Google 検索" />
          <input class="btn lucky-btn" value="I'm Feeling Lucky" />
        </div>
      </div>
      <footer>
        <div class="footer1">
          <div class="country">
            日本
          </div>
        </div>
        <div class="footer2">
          <ul class="footer2-left">
            <li><a href="#">広告</a></li>
            <li><a href="#">ビジネス</a></li>
            <li><a href="#">Googleについて</a></li>
            <li><a href="#">検索の仕組み</a></li>
          </ul>
          <ul class="footer2-right">
            <li><a href="#">プライバシー</a></li>
            <li><a href="#">規約</a></li>
            <li><a href="#">設定</a></li>
          </ul>
        </div>
      </footer>
    </div>
  </div>
</template>

<style>
.container {
  width: 100%;
}
li {
  list-style: none;
}
a {
  text-decoration: none;
  color: #555555;
}
header {
  width: 100%;
  height: 60px;
  position: absolute;
  top: 0;
  font-size: 14px;
  line-height: 60px;
}
header .header-menu {
  float: right;
  margin-right: 20px;
}
header .header-menu li {
  float: left;
  margin: 0 10px;
}
header .header-menu li:hover {
  text-decoration: underline;
  opacity: 0.9;
}
.appli-icon {
  width: 20px;
  height: 20px;
  background-color: #999999;
  margin: 20px 0;
}
.user-icon {
  width: 30px;
  border-radius: 30px;
  margin-top: 15px;
}
.main {
  width: 500px;
  margin: 180px auto;
  text-align: center;
}
h1 {
  font-size: 80px;
  font-weight: bold;
  letter-spacing: -10px;
}
.blue {
  color: #4285f4;
}
.red {
  color: #eb4335;
}
.yellow {
  color: #fcbc05;
}
.green {
  color: #33a853;
}
.search {
  width: 100%;
}
.search input {
  padding: 5px 20px;
  margin-top: 30px;
  line-height: 2.5;
}
.search-box {
  width: 100%;
  border: 2px solid #e6e6e6;
  border-radius: 30px;
}
.search-box:hover {
  box-shadow: 0px 2px 6px #999999;
}
.btns {
  margin: 0 auto;
}
.search .btn {
  text-align: center;
  width: 30%;
  box-sizing: border-box;
  line-height: 2;
  font-size: 13px;
  border-radius: 4px;
  background-color: #f2f2f2;
  border: 1px solid #f2f2f2;
}
.search .btn:hover {
  border: 1px solid #c9c9c9;
  cursor: pointer;
}
footer {
  width: 100%;
  background-color: #f2f2f2;
  position: absolute;
  bottom: 0;
  font-size: 13px;
  line-height: 3;
}
footer .footer1 {
  border-bottom: 1px solid #e6e6e6;
  padding-left: 30px;
  font-size: 15px;
  color: #555555;
}
.footer2-left {
  padding-left: 20px;
}
.footer2-left li {
  float: left;
  margin: 0 13px;
}
.footer2-left li:hover {
  text-decoration: underline;
}
.footer2-right {
  padding-right: 20px;
  float: right;
}
.footer2-right li {
  float: left;
  margin: 0 13px;
}
.footer2-right li:hover {
  text-decoration: underline;
}
</style>
