<template>
  <el-col :span="4">
    <el-card class="box-card">
      <div slot="header">
        <span>Свободные вакансии</span>
      </div>
      <div v-for="item in vacancies">
        {{item.vacancy}}
        {{ item.amount}}
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
