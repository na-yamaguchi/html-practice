<template>
  <div class="container">
    <header>
      <ul class="header-menu">
        <li><a href="#">Gmail</a></li>
        <li><a href="#">画像</a></li>
        <li>
          <a href="#">
            <div class="app-icon" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/myicon.jpg" class="user-icon" />
          </a>
        </li>
      </ul>
    </header>
    <main>
      <h1>
        <span class="blue">G</span>
        <span class="red">o</span>
        <span class="yellow">o</span>
        <span class="blue">g</span>
        <span class="green">l</span>
        <span class="red">e</span>
      </h1>
      <div class="search">
        <div class="search-box">
          <input type="text" />
          <img src="/mic-icon.svg" class="mic-icon" />
        </div>
        <div class="voice-input">音声で検索</div>
      </div>
      <div class="buttons">
        <button class="search-button">Google 検索</button>
        <button class="lucky-button">I'm Feeling Lucky</button>
      </div>
    </main>
    <footer>
      <div class="region-footer">
        <div class="country">
          日本
        </div>
      </div>
      <div class="menu-footer">
        <ul class="about">
          <li><a href="#">広告</a></li>
          <li><a href="#">ビジネス</a></li>
          <li><a href="#">Googleについて</a></li>
          <li><a href="#">検索の仕組み</a></li>
        </ul>
        <ul class="rule">
          <li><a href="#">プライバシー</a></li>
          <li><a href="#">規約</a></li>
          <li><a href="#">設定</a></li>
        </ul>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
ul {
  list-style: none;
  padding: 0;
}

a {
  text-decoration: none;
  color: #555555;

  &:hover {
    text-decoration: underline;
    opacity: 0.9;
  }
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;

  header {
    width: 100%;
    height: 60px;
    font-size: 14px;
    line-height: 60px;

    ul {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      margin-right: 20px;

      li {
        margin: 0 10px;
      }

      .app-icon,
      .user-icon {
        width: 30px;
        height: 30px;
        line-height: 60px;
        vertical-align: middle;
      }

      .app-icon {
        display: inline-block;
        background-color: gray;
      }

      .user-icon {
        border-radius: 50%;
      }
    }
  }

  main {
    width: 100%;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    h1 {
      font-size: 80px;
      letter-spacing: -10px;

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
    }

    .search {
      position: relative;

      .search-box {
        border: 1px solid #e4e4e4;
        border-radius: 30px;
        padding: 0 10px 0 20px;
        margin-top: 30px;

        &:hover {
          box-shadow: 0px 2px 6px #999999;
        }

        input {
          line-height: 2.5;
          font-size: 14px;
          border-style: none;
          width: 400px;

          &:focus {
            outline: none;
          }
        }

        .mic-icon {
          position: relative;
          top: 5px;
          display: inline-block;
        }
      }

      .voice-input {
        display: inline-block;
        font-size: 11px;
        background-color: #2d2d2d;
        color: #ffffff;
        padding: 5px;
        border-radius: 2px;
        position: absolute;
        right: -10px;

        &::before {
          content: "";
          border: 5px solid transparent;
          border-bottom: 5px solid #2d2d2d;
          position: absolute;
          top: -10px;
          right: 42%;
          z-index: 2;
        }
      }
    }

    .buttons {
      margin-top: 20px;

      button {
        line-height: 2;
        font-size: 13px;
        border-radius: 4px;
        background-color: #f2f2f2;
        border: 1px solid #f2f2f2;
        padding: 5px 15px;
        margin: 0 5px;

        &:hover {
          border: 1px solid #c9c9c9;
          cursor: pointer;
          opacity: 0.9;
        }

        &:focus {
          outline: none;
        }
      }
    }
  }

  footer {
    width: 100%;
    height: auto;
    background-color: #f2f2f2;
    font-size: 15px;
    line-height: 3;
    border-top: 1px solid #e4e4e4;

    .region-footer {
      margin: 0 32px;
      color: #555555;
    }

    .menu-footer {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      border-top: 1px solid #e4e4e4;

      ul {
        display: flex;
        font-size: 13px;
        margin: 0 20px;
      }

      li {
        margin: 0 12px;
      }
    }
  }
}
</style>
