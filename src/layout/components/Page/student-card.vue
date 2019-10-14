<template>
  <el-col :span="8">
  <el-card class="box-card">
    <div slot="header" class="clearfix">
      <span>Статистика</span>
    </div>
    <div>
      <el-row gutter="20">
        <el-col>
<!--         :span="4">-->
            <el-row v-for="item in items" style="line-height: 1.5">
              <el-col :span="20"> {{ item.key }}</el-col>
              <el-col :span="4" style="text-align: right"> {{ item.value }}</el-col>
            </el-row>
        </el-col>
<!--        <el-col :span="14">-->
<!--          <p>graph</p>-->
<!--        </el-col>-->
      </el-row>
    </div>
  </el-card>
  </el-col>
</template>

<script>
    export default {
        name: "studentCard",
        data() {
            return {
              items: [
                  {key: 'Активные задачи:', value: '2'},
                  {key: 'Выполненные задачи: ', value: '1'},
                  {key: 'Зачтенные часы:', value: '12'},
                  {key: 'Осталось часов:', value: '138'},
              ]
            }
        }
    }
</script>

<style scoped>
  body {
    margin-bottom: 60px;
  }

  .el-col {
    height: 100% ;
  }

  .el-card {
    height: 100% !important;
  }
</style>
