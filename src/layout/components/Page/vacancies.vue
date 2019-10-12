<template>
  <el-col :span="6">
    <el-card class="box-card">
      <div slot="header">
        <span>Свободные вакансии</span>
      </div>
      <div v-for="item in vacancies">
        <el-row style="line-height: 1.5">
          <el-col :span="20">{{item.vacancy}}</el-col>
          <el-col :span="4" style="text-align: right"> {{ item.amount}}</el-col>
        </el-row>

      </div>
    </el-card>
  </el-col>
</template>

<script>
    export default {
        name: "vacancies",
        data() {
            return {
                vacancies: [{vacancy: 'Frontend', amount: 2},
                    {vacancy: 'Frontend', amount: 2},
                    {vacancy: 'Frontend', amount: 2},
                ]
            }
        }
    }
</script>

<style scoped>


</style>
