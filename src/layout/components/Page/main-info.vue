<template>
  <el-row class="row-margin-bottom">
    <el-col :span="22">
      <el-row class="info">
          <span class="project-id">{{ id }}</span>
          <el-tag color="#C6F0EE">
            {{ type }}
          </el-tag>
      </el-row>
      <el-row>
        <h1>{{ nameRus }}</h1>
        <h3>{{ nameEng }}</h3>
      </el-row>
    </el-col>
    <el-col :span="2">
      <div class="links">
      <a class="icon-link" href="https://trello.com/" target="_blank">
        <img src="../../../assets/404_images/trello.svg" alt="Trello">
      </a>
      <a class="icon-link" href="https://git.miem.hse.ru/" target="_blank">
        <img src="../../../assets/404_images/git.svg" alt="Git" >
      </a>
        </div>
    </el-col>
  </el-row>
</template>

<script>
    export default {
        name: 'mainInfo',
        data() {
            return {
                id: '№199212',
                type: 'программно-аппаратный',
                nameRus: 'Сервисы цифровой интегрированной среды',
                nameEng: 'Digital Integrated Services'
            }
        },
        methods: {}
    }
</script>

<style scoped>
  .el-row {
    height: auto;
    line-height: normal;
  }

  .el-col {
    text-align: left;
  }

  .icon-link {
    display: block;
    width: 42px;
    height: 42px;
    margin-bottom: 12px;
  }

  span.project-id {
    margin-right: 12px;
    font-size: 16px;
    font-weight: bold;
    color: #797878;
  }

  .info div {
    display: inline-block;
  }

  div.links {
    float: right;
  }

  h1 {
    margin-top: 20px;
    margin-bottom: 12px;
    font-size: 44px;
    font-weight: bold;
    word-wrap: normal;
    text-align: left;
    line-height: normal;
  }

  h3 {
     font-size: 20px;
     font-weight: bold;
     word-wrap: normal;
     text-align: left;
     line-height: normal;
     color: #797878;
   }

  span.project-id {
    margin: 0px 12px 0px 0px;
    font-size: 18px;
    font-weight: normal;
    text-align: left;
    line-height: normal;
    color: #797878;
  }

  .el-tag {
    font-size: 14px;
    border-color: #C6F0EE;
    color: #000000;
  }

  body {
    margin-bottom: 60px;
  }

  img {
    width: 42px;
    height: 42px;
  }

</style>
