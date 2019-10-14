<template>
  <el-col :span="4" class="main-col">
    <h5>Навигация</h5>
    <el-menu class="main-menu">
      <el-menu-item index="1">
        <a href="#main-info">
        <span>Основная информация</span>
        </a>
      </el-menu-item>

      <el-submenu index="2">
        <template slot="title">
          <span>Детали проекта</span>
        </template>

          <el-menu-item  class="sub" v-for="(item,index) in items" index="2-1">
            <a v-bind:href="'#' + index">
              {{item.key}}
            </a>
          </el-menu-item>

      </el-submenu>

      <el-menu-item index="3">
        <a href="#vacancies">
          <span>Вакансии</span>
        </a>
      </el-menu-item>

      <el-menu-item index="4">
        <a href="#student-card">
          <span>Моя статистика</span>
        </a>
      </el-menu-item>

      <el-submenu index="5">
        <template slot="title">
        <span>Состав проекта</span>
        </template>
        <el-menu-item class="sub" index="4-1"> <a href="#heads">Руководители</a></el-menu-item>
        <el-menu-item class="sub" index="4-2"><a href="#students">Студенты</a></el-menu-item>
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
                ],
            }
        }
    }
</script>

<style scoped>

  .sub {
    height: auto;
    line-height: 1.15;

    white-space: normal;
    padding: 18px 0;
  }

  .main-col {
    position: fixed;
    padding-right: 10px;
  }

  .main-menu {
    border-right-color: transparent;
    word-wrap: normal;
  }

  .el-menu-item a {
    display: block;
  }

  h5 {
    padding-left: 20px;
    margin: 15px 0;
    font-size: 18px !important;
  }

</style>
