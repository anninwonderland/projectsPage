<template>
  <el-row class="row-margin-bottom">
    <el-col :span="24">
      <h4>Детали проекта</h4>
      <el-collapse>
        <el-collapse-item :id=index v-for="(item,index) in items"
                          v-bind:title="item.key">
          <div class="desc">
            {{item.description}}
          </div>
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
