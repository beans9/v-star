<template>
  <div class="main">
    <main>
      <header>
        <div class="wrapper">
            <div class="header-left">
              <a href="" class="header-left-logo-a"><div class="header-left-logo"></div></a>
            </div>
            <div class="header-center">
              <div class="header-center-search-layout">
                <div class="header-center-search-icon"></div>
                <span>검색</span>
              </div>
            </div>
            <div class="header-right">
              <a href="" class="header-right-a"><div class="header-right-menu1"></div></a>
              <a href="" class="header-right-a"><div class="header-right-menu2"></div></a>
              <a href="" class="header-right-a"><div class="header-right-menu3"></div></a>
            </div>
        </div>
      </header>
      <div class="profile">
        <div class="profile-image">
          <img src="~@/assets/aa.png" class="profile-image-logo" />
        </div>

        <section class="profile-desc">
          <div class="prifile-desc-title">
            <h1>abcd</h1>
            <span class="auth-badge">인증됨</span>
            <span class="button-layout">
              <button class="button blue long">팔로우</button>
              <button class="button blue"><div class="btn-down-arrow"></div></button>
              <button class="button transparent"><div class="btn-more"></div></button>
            </span>
          </div>
          <ul class="profile-desc-ul">
            <li>
              <span>게시물
                <span class="strong">178</span>
              </span>
            </li>
            <li>
              <span>팔로워
                <span class="strong">178</span>
              </span>
            </li>
            <li>
              <span>팔로워
                <span class="strong">178</span>
              </span>
            </li>
          </ul>
          <div class="profile-desc-detail">
            <h1>abcd</h1>
            <span>The official Instagram for ABCd 🙅🏽🦄🤗 Your source for digital original series ft. up-and-coming talent and established voices. Tap that app
  abc.tv/2hzE3IU</span>
          </div>
        </section>
      </div>
      <div class="list">
        <ul class="list-ul">
          <li v-for="(item,index) in list" v-bind:key="index">
            <div class="content">
              <img src="~@/assets/qqq.png" />
              {{item}}
            </div>
          </li>
        </ul>
      </div>
    </main>
    <footer>
      <ul class="footer-ul">
        <li><a href="">소개</a></li>
        <li><a href="">지원</a></li>
        <li><a href="">블로그</a></li>
        <li><a href="">홍보센터</a></li>
        <li><a href="">API</a></li>
        <li><a href="">채용정보</a></li>
        <li><a href="">개인정보보호</a></li>
        <li><a href="">약관</a></li>
      </ul>
      <p>© 2018 Instagram</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'Main',
  data () {
    return {
      msg: 'Main Page',
      list: [1, 2, 3, 4, 5]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body {
  background-color: #fafafa;
}

.main {
  height:100vh;
  min-height:500px;
  display:flex;
  flex-direction: column;
}

main {
  display:flex;
  flex:1 0 auto;
  flex-direction:column;
}

h1, h2 {
  font-weight: normal;
  margin: 0;
}

header {
  background-color: white;
  height: 77px;
  line-height: 77px;
  border-bottom: 1px solid rgba(0,0,0,.0975);
}

.header-left,.header-right,.header-center {
  display:inline-block;
}

.header-left {
  float:left;
}
.header-left-logo-a {
  display:inline-block;
  vertical-align: middle;
}

.header-left-logo {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -177px -264px;
  height: 35px;
  width: 176px;
  vertical-align:middle;
}

.header-right {
  float:right;
}

.header-right-a {
  display:inline-block;
  vertical-align: middle;
}

.header-right-a + .header-right-a {
  margin-left: 25px;
}

.header-right-menu1 {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -335px -399px;
  height: 24px;
  width: 24px;
}

.header-right-menu2 {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -257px -399px;
  height: 24px;
  width: 24px;
}

.header-right-menu3 {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -182px -479px;
  height: 24px;
  width: 24px;
}

.header-center-search-layout {
  border: solid 1px #dbdbdb;
  border-radius: 3px;
  color: #999;
  font-size: 14px;
  outline: 0;
  padding: 3px 10px 3px 10px;
  z-index: 2;
  width:215px;
  height:28px;
  line-height:22px;
  box-sizing: border-box;
  displaY:inline-block;
  vertical-align: middle;
  background-color: #fafafa;
}

.header-center-search-icon {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -429px -385px;
  height: 10px;
  width: 10px;
  display:inline-block;
}

.wrapper {
  width: 953px;
  margin: 0 auto;
}

.profile {
  width: 953px;
  margin: 0 auto;
  /* background-color: red; */
  margin-top:30px;
}

.profile-image {
  display:inline-block;
  width:30%;
  text-align: center;
  /* border:1px solid blue; */
  vertical-align: top;
}

.profile-image-logo {
  width:152px;
  height:152px;
  border-radius: 75px;
}

.profile-desc {
  width:65%;
  text-align: left;
  display:inline-block;
}

.prifile-desc-title h1 {
  display:inline-block;
  font-size: 32px;
  line-height: 40px;
  font-weight: 200;
}

.profile-desc-detail {
  font-size: 16px;
  line-height: 24px;
}

.profile-desc-detail h1 {
  font-size: 16px;
  font-weight: bold;
  display:inline-block;
}

.button-layout {
  vertical-align: super;
}

.button {
  border-color:#dbdbdb;
  border-radius: 3px;
  color:white;
  padding: 0 10px;
  font-size:14px;
  height:28px;
  display:inline-block;
  margin-left:5px;
  vertical-align: bottom;
  margin-bottom:5px;
  cursor: pointer;
}

.blue {
  background-color:#3897f0;
  border-color:#3897f0;
}

.button.long {
  padding: 0 20px;
}

.button.transparent {
  border-color: transparent !important;
  padding: 0;
}

.auth-badge {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -546px -179px;
  height: 18px;
  width: 18px;
  display: block;
  overflow: hidden;
  text-indent: 110%;
  white-space: nowrap;
  display: inline-block;
}

.btn-down-arrow {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -453px -385px;
  width: 9px;
  height: 6px;
}

.btn-more {
  background-image: url('../assets/instargram.png');
  background-repeat: no-repeat;
  background-position: -546px -336px;
  height: 16px;
  width: 16px;
}

.profile-desc {
  height: auto;
}

.profile-desc-ul {
  padding-left: 0px;
}

.profile-desc-ul li {
  list-style: none;
  display:inline-block;
  width:20%;
  text-align: left;
}

.list {
  /* background-color: blue; */
  width: 953px;
  margin:0 auto;
  padding-top:40px;
}

.list-ul {
  padding: 0;
  margin: 0;
  text-align: left;
  font-size:0;
}

.list-ul li {
  font-size:1rem;
  /* background-color: yellow; */
  list-style:none;
  display:inline-block;
  width:33.3%;
  text-align:center;
  margin-top:9px;
  /* border:1px solid red; */
  box-sizing: border-box;
  padding:5px;
}

li:nth-child(3n) {
  margin-right:0;
}

.content {
  width:100%;
  height:100%;
  font-size:1rem;
  color:white;
}

.content img {
  width: 293px;
  height: 293px;
}

footer {
  height:50px;
  width: 953px;
  margin: 0 auto;
  /* background-color: green; */
  text-align: left;
  font-size:12px;
  padding: 5px;
  font-weight: 600;
  text-transform: uppercase;
  box-sizing: border-box;
  margin-bottom:30px;
}

.footer-ul {
  display:inline-block;
  padding-left: 0;
}

.footer-ul li {
  display:inline-block;
  list-style: none;
  margin-right: 15px;
}

.footer-ul li a {
  text-decoration: none;
  color: #003569;
}

footer p {
  float:right;
}

.strong {
  font-weight: bold;
}
</style>
