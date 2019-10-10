<template>
  <el-row :span="24">
  <el-card class="box-card">
    <div slot="header" class="clearfix">
      <span>Статистика</span>
    </div>
    <div v-for="item in items"  class="text item">
      <el-col> {{ item.key }}</el-col>
      <el-col> {{ item.value }}</el-col>
    </div>
  </el-card>
  </el-row>
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
</style>
