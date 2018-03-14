<template>
  <div class="main">
    <header>인스타그램 검색 메뉴</header>
    <div class="profile">
      프로필
    </div>
    <div class="list">
      <ul>
        <li>
          <div class="content">
            1
          </div>
        </li>
        <li>
          <div class="content">
            1
          </div>
        </li>
        <li>
          <div class="content">
            1
          </div>
        </li>
        <li>
          <div class="content">
            1
          </div>
        </li>
        <li>
          <div class="content">
            1
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
  data () {
    return {
      msg: 'Main Page'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

header {
  background-color: green;
}

.profile {
  background-color: red;
}

.list {
  background-color: blue;
  width: 953px;
  margin:0 auto;
}

ul {
  padding: 0;
  margin: 0;
  text-align: left;
  font-size:0;
}

li {
  font-size:1rem;
  background-color: yellow;
  list-style:none;
  display:inline-block;
  width:33.3%;
  text-align:center;
  margin-top:20px;
  border:1px solid red;
  box-sizing: border-box;
  padding:5px;
}

li:nth-child(3n) {
  margin-right:0;
}

.content {
  width:100%;
  height:100%;
  background-color:purple;
  font-size:1rem;
  color:white;
}
</style>
