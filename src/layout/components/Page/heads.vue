<template>
  <el-row class="row-margin-bottom">
  <el-col span="24">
    <h5>Руководители</h5>
  <el-table
    :data="headsData"
    border
    style="width: 100%">
    <el-table-column
      prop="role"
      label="Должность"
      >
    </el-table-column>
    <el-table-column
      prop="name"
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
                    role: 'руководитель направления',
                    name: 'Иванов Иван Иванович',
                    link: 'www.wikipedia.org',
                    email: 'ivanovii@hse.ru',
                    phone: '+7-999-888-77-22',

                },
                    {
                        role: 'руководитель направления',
                        name: 'Иванов Иван Иванович',
                        link: 'www.wikipedia.org',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',

                    },
                    {
                        role: 'руководитель направления',
                        name: 'Иванов Иван Иванович',
                        link: 'www.wikipedia.org',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',

                    },
                    {
                        role: 'руководитель направления',
                        name: 'Иванов Иван Иванович',
                        link: 'www.wikipedia.org',
                        email: 'ivanovii@hse.ru',
                        phone: '+7-999-888-77-22',

                    }]

            }
        }
    }
</script>

<style scoped>

</style>
