<template>
  <div class="app-container">
    <el-container>
      <el-aside width="180px">
        <sidebar></sidebar>
      </el-aside>

      <el-container>
        <el-main>
          <main-info></main-info>
          <info></info>
          <student-card></student-card>
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
import students from "../../layout/components/Page/students.vue";
import sidebar from "../../layout/components/Page/sidebar.vue";

export default {
    components: {mainInfo, info, studentCard, heads, students, sidebar},
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
  height: auto;

}
.el-main {
  margin: 10px 40px 0px 40px;
}

body > .el-container {
  margin-bottom: 40px;
}
</style>

