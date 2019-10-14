<template>
  <el-row class="row-margin-bottom">
  <el-col span="24">
    <h4>Состав проекта</h4>
    <h5>Руководители</h5>
  <el-table
    :data="headsData"
    border
    style="width: 100%">
    <el-table-column
      fit="true"
      prop="role"
      label="Должность"
      >
    </el-table-column>
    <el-table-column
      prop="name"
      width="220px"
      label="ФИО"
      >
    </el-table-column>
    <el-table-column
      prop="link"
      label="Профиль">
    </el-table-column>
    <el-table-column
      prop="email"
      label="Электронная почта">
    </el-table-column>
    <el-table-column
      prop="phone"
      width="160px"
      label="Телефон">
    </el-table-column>
  </el-table>
  </el-col>
    </el-row>
</template>

<script>
    export default {
        name: "heads",
        data() {
            return {
                headsData: [{
                    role: 'руководитель',
                    name: 'Иванов Иван Иванович',
                    link: 'www.wikipedia.org',
                    email: 'ivanovii@hse.ru',
                    phone: '+7-999-888-77-22',

                },
                    {
                        role: 'руководитель',
                        name: 'Петров Иван Иванович',
                        link: 'www.wikipedia.org',
                        email: 'petrov@hse.ru',
                        phone: '+7-999-128-71-10',

                    },
                    {
                        role: 'куратор направления',
                        name: 'Масленкин Ян Игоревич',
                        link: 'www.wikipedia.org',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-784-44-42',

                    },
                    ]

            }
        }
    }
</script>

<style scoped>

</style>
