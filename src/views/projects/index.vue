<template>
  <div class="app-container">
    <el-container>
      <el-aside width="180px">Aside</el-aside>
      <el-container>
        <el-main>
          <main-info></main-info>
          <student-card></student-card>
          <info></info>
          <heads></heads>
          <students></students>
        </el-main>
      </el-container>
    </el-container>

  </div>
</template>

<script>
import mainInfo from '../../layout/components/Page/main-info.vue'
import studentCard from '../../layout/components/Page/student-card.vue'
import info from '../../layout/components/Page/info.vue'
import heads from '../../layout/components/Page/heads.vue'
import students from "../../layout/components/Page/students";

export default {
    components: {mainInfo, info, studentCard, heads, students},
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
  line-height: normal;
}
.el-main {
  color: #333;
  line-height: normal;
  margin: 40px 40px 0px 40px;

}

body > .el-container {
  margin-bottom: 40px;
}
</style>

