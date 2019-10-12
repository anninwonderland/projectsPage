<template>
  <el-row class="row-margin-bottom">
  <el-col span="24">
    <h5>Студенты</h5>
    <el-table
    :data="studentsData"
    border
    style="width: 100%">
    <el-table-column
      prop="role"
      label="Роль в проекте"
      sortable
      >
    </el-table-column>
    <el-table-column
      prop="name"
      label="ФИО"
      >
    </el-table-column>
    <el-table-column
      prop="group"
      label="Группа">
    </el-table-column>
    <el-table-column
      prop="email"
      label="Электронная почта">
    </el-table-column>
    <el-table-column
      prop="phone"
      label="Телефон">
    </el-table-column>
  </el-table>
  </el-col>
    </el-row>
</template>

<script>
    export default {
        name: "students",
        data() {
            return {
                studentsData: [{
                    role: 'фронтенд',
                    name: 'Иванов Иван Иванович',
                    group: 'БИВ-174',
                    email: 'ivanovii@hse.ru',
                    phone: '+7-999-888-77-22',
                },
                    {
                        role: 'фронтенд',
                        name: 'Иванов Иван Иванович',
                        group: 'БИВ-174',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',
                    },
                    {
                        role: 'фронтенд',
                        name: 'Иванов Иван Иванович',
                        group: 'БИВ-174',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',
                    },
                    {
                        role: 'фронтенд',
                        name: 'Иванов Иван Иванович',
                        group: 'БИВ-174',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',
                    },
                    {
                        role: 'фронтенд',
                        name: 'Иванов Иван Иванович',
                        group: 'БИВ-174',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',
                    },
                ]
            }
        }
    }
</script>

<style scoped>

</style>
