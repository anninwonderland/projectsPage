<template>
  <div class="app-container">
    <el-container>
      <el-row class="main">
        <el-col span="4">
          <el-aside width="200px">
            <sidebar></sidebar>
          </el-aside>
        </el-col>
        <el-col span="20" offset="4">

          <el-main>

              <main-info></main-info>
              <info></info>

            <el-row>
              <vacancies></vacancies>
              <student-card></student-card>
            </el-row>

              <heads></heads>


              <students></students>

          </el-main>

        </el-col>
      </el-row>
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
    import vacancies from "../../layout/components/Page/vacancies.vue";

    export default {
        components: {mainInfo, info, studentCard, heads, students, sidebar, vacancies},
        data() {
            return {}
        },
        methods: {}
    }
</script>

<style>

  .el-aside {
    background-color: #D3DCE6;
    height: 100%;
    position: fixed;
  }

  .el-main {
  }

  .main {
    width: 100%;
  }

</style>

