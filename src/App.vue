<template>
  <div id="app">
    <el-container>
      <el-header height="90px">
        <el-row>
          <el-col :span="4">
            <div class="grid-content bg-purple">
               <img src="./assets/logo-head.png">
            </div>
          </el-col>
          <el-col :span="16"><div class="grid-content bg-purple-light"></div></el-col>
          <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
        </el-row>
      </el-header>
      <el-main>
        <router-view/>
      </el-main>
      <el-footer height="30px">
        <el-row>
          <el-col :span="24"><div class="footer">Copyright©2013</div></el-col>
        </el-row>
      </el-footer>
    </el-container>
    
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
}
.el-header, .el-footer {
  background-color: #409EFF;
  color: #333;
  text-align: center;
  height: 90px;
}
.el-main {
  background-color: #E9EEF3;
  color: #333;
  text-align: center;
  height: calc(100vh - 120px);
}
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .footer{
    height: 30px;
    line-height: 30px;
  }
</style>
