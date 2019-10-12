<template>
  <el-row>
    <el-col :span="24">
      <el-collapse v-for="item in items">
        <el-collapse-item v-bind:title="item.key">
          <div class="desc">{{item.description}}</div>
        </el-collapse-item>
      </el-collapse>
    </el-col>
  </el-row>
</template>


<script>
    export default {
        name: "info",
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

</style>
