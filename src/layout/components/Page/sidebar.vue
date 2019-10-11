<template>
  <el-col :span="4">
    <h5>Навигация</h5>
    <el-menu>
      <el-menu-item index="1">
        <span>Основная информация</span>
      </el-menu-item>

      <el-submenu index="2">
        <template slot="title">
          <span>Детали проекта</span>
        </template>
        <div v-for="item in items">
          <el-menu-item index="2-1"> {{item.key}}</el-menu-item>
        </div>
      </el-submenu>

      <el-menu-item index="3">
        <el-badge type="success" value="!" class="item">
        <span>Моя статистика</span>
        </el-badge>
      </el-menu-item>

      <el-submenu index="4">
        <template slot="title">
        <span>Состав проекта</span>
        </template>
        <el-menu-item index="4-1">Руководители</el-menu-item>
        <el-menu-item index="4-2">Студенты</el-menu-item>
      </el-submenu>

    </el-menu>
  </el-col>
</template>

<script>
    export default {
        name: "sidebar",
        data() {
            return {
                items: [
                    {key: 'Цель проекта', description: 'Сделать что-то'},
                    {key: 'Ожидаемые результаты', description: 'готовое что-то'},
                    {key: 'Описание проекта', description: 'Сделать что-то'},
                    {key: 'Карта компетенций', description: 'Что-то тут еще такое'},
                    {key: 'Ресурсное обеспечение', description: 'Что-то интересное'},
                    {key: 'Форма и способы промежуточного контроля', description: 'Что-то еще интересное'},
                    {key: 'Форма представления результатов', description: 'И тут тоже'},
                ]
            }
        }
    }
</script>

<style scoped>

  .el-menu-item {
    word-wrap: normal;
  }
</style>
