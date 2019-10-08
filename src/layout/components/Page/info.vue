<template>
  <el-col :span="24">
    <el-row>
      <el-col class="item" :span="4"> {{ item }}</el-col>
      <el-col class="description" :span="20"> {{ description }}</el-col>
    </el-row>
    <el-divier></el-divier>
    <el-row>
      <el-col class="item" :span="4"> {{ item }}</el-col>
      <el-col class="description" :span="20"> {{ description }}</el-col>
    </el-row>
    <el-divier></el-divier>
    <el-row>
      <el-col class="item" :span="4"> {{ item }}</el-col>
      <el-col class="description" :span="20"> {{ description }}</el-col>
    </el-row>
    <el-divier></el-divier>
    <el-row>
      <el-col class="item" :span="4"> {{ item }}</el-col>
      <el-col class="description" :span="20"> {{ description }}</el-col>
    </el-row>
    <el-divier></el-divier>
  </el-col>

</template>

<script>
    export default {
        name: "info",
        data() {
            return {
                item: "Описание проекта:",
                description: "Необходимо спроектировать онлайн-инструмент – единую точку. Проект необходим для того, чтобы то и чтобы это.",
            }
        }
    }
</script>

<style scoped>

  .el-col {
    margin: 20px 0px 20px 0px;
    text-align: left;
    line-height: 18px;
    align-content: center;
    word-wrap: normal;
    font-size: 16px;
  }

  .item {
    font-weight: bold;
    color: #797878;
  }

  .description {
    padding-left: 40px;
  }

  /*p {*/
  /*  text-align: left;*/
  /*  font-size: 24px;*/
  /*  font-weight: bold;*/
  /*  font-family: "Helvetica Neue", Helvetica, "PingFang SC", Arial, sans-serif;*/
  /*  line-height: normal;*/
  /*  color: #797878;*/
  /*}*/

  /*.description {*/
  /*  font-size: 20px;*/
  /*}*/
</style>
