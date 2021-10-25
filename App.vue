<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view/>
    <h2>编辑岗位</h2>     
      <div class="l l_list"> 
        <p>归属部门:</p>
        <select id='checkedList'>
　　　  　 <option value='' disabled selected style='display:none;'>和智数据/技术总/前端</option>
          <option value="和智数据">和智数据</option>
　　　　   <option value="技术总">技术总</option>
　　　　   <option value="前端">前端</option>                                                                                                                                                          
　　     </select> 
        <p>岗位名称:</p>
        <input type="text" id='workName' value="123">
      </div>
      <div class="l r_list"> 
          <p>可授权的角色:</p>
          <div class="table">
            <ul>
              <li>
                <p>名称</p>|
                <p>描述</p>
              </li>
              <li>
                <i class="iconfont icon-xiala"></i>
                <p></p>
              </li>
            </ul>
          </div>
      </div>
    </div>
 
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
*{margin:0;padding: 0;}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 15px auto;
  background-color: #E5F5FF;
  width: 800px;
  height: 600px;
}
h2{
  font-weight: normal;
  /* background-color: white; */
  padding: 5px;
}
p{
  font-size: 16px;
}
.l{
  float: left;
}
.r{
  float: right;
}
.l_list{
  text-align: left;
  height: 100%;
  width: 250px;
  background-color: blanchedalmond;
  
}
#checkedList{
  width:200px;
  height:25px;
  outline:none;
}
input{
  width:195px;
  height:20px;
  outline:none;
}
.r_list{
  text-align: left;
  height: 100%;
  width: 80px;
  background-color: red;
}
ul{
  list-style: none;
}
</style>
