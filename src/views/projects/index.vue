<template>
  <div class="app-container">
    <el-container>
      <el-row class="main-row row-margin-bottom"
              gutter="10">
        <el-col span="4">
          <el-aside>
            <sidebar></sidebar>
          </el-aside>
        </el-col>
        <el-col span="20" offset="4">
          <el-main>
              <main-info id="main-info"></main-info>
              <info></info>

            <el-row class="row-margin-bottom cards-in-row"
                    gutter="20">
              <vacancies id="vacancies"></vacancies>
              <student-card id="student-card"></student-card>
            </el-row>

              <heads id="heads"></heads>


              <students id="students"></students>

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
  }

  .el-main {
  }

  .row-margin-bottom {
    margin-bottom: 20px;
  }

  .row-margin-bottom:last-child {
     margin-bottom: 0;
  }

  .cards-in-row .el-col {
    height: 100%;
  }
  .main-row {
    width: 100%;
  }


</style>

