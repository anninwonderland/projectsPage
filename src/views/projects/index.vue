<template>
  <div class="app-container">
    <el-container>
      <el-aside width="180px">Aside</el-aside>
      <el-container>
        <el-main>
          <main-info></main-info>
          <info></info>
        </el-main>
      </el-container>
    </el-container>

  </div>
</template>

<script>
import mainInfo from '../../layout/components/Page/main-info.vue'
import info from '../../layout/components/Page/info.vue'
export default {
    components: {mainInfo, info},
  data() {
    return {
    }
  },
  methods: {
  }
}
</script>

<style>

.el-aside {
  background-color: #D3DCE6;
  color: #333;
  text-align: center;
  line-height: normal;
}
.el-main {
  color: #333;
  text-align: center;
  line-height: normal;
  margin: 40px 40px 0px 40px;

}

body > .el-container {
  margin-bottom: 40px;
}
</style>

