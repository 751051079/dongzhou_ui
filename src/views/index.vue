<template>
  <div class="app-container home">
    <el-row :gutter="20">
      <el-col :sm="24" :lg="12" style="padding-left: 20px">
        <h2>东洲科技后台管理ERP</h2>
        <p>
          &nbsp;&nbsp;&nbsp;&nbsp;东洲科技后台管理 ERP 系统是一套基于 RuoYi-Vue 框架 开发的企业级后台管理平台，集成了 用户权限管理、系统配置、数据可视化
          等基础功能。在此基础上，系统重点扩展了
          美可多业务管理模块，实现了与美可多平台对接的核心功能，包括：
        </p>
        <p><strong>&nbsp;&nbsp;&nbsp;&nbsp;刊登管理：</strong>支持商品的批量刊登、编辑与上下架，提升运营效率。</p>

        <p><strong>&nbsp;&nbsp;&nbsp;&nbsp;订单管理：</strong>实时同步美可多平台订单信息，支持订单查询、发货处理与状态跟踪。</p>

        <p><strong>&nbsp;&nbsp;&nbsp;&nbsp;库存管理：</strong>对接平台库存接口，确保商品库存与平台保持一致，避免超卖或缺货。</p>

        <p><strong>&nbsp;&nbsp;&nbsp;&nbsp;数据分析：</strong>结合 ERP 系统数据统计能力，为运营决策提供可视化支持。</p>

        <p>
          &nbsp;&nbsp;&nbsp;&nbsp;系统采用 前后端分离架构（前端 Vue 3 + Element Puls，后端 Spring Boot + MyBatis + Redis + MySQL），具备
          高扩展性、可维护性和良好的用户体验，能够为企业在美可多平台上的运营管理提供高效、稳定的支撑。
        </p>
        <p>
          <b>当前版本:</b> <span>v{{ version }}</span>
        </p>
      </el-col>

      <el-col :sm="24" :lg="12" style="padding-left: 50px">
        <el-row>
          <el-col :span="12">
            <h2>技术选型</h2>
          </el-col>
        </el-row>
        <el-row>
          <el-col :span="6">
            <h4>后端技术</h4>
            <ul>
              <li>SpringBoot</li>
              <li>Spring Security</li>
              <li>JWT</li>
              <li>MyBatis</li>
              <li>Druid</li>
              <li>Fastjson</li>
              <li>...</li>
            </ul>
          </el-col>
          <el-col :span="6">
            <h4>前端技术</h4>
            <ul>
              <li>Vue</li>
              <li>Vuex</li>
              <li>Element-ui</li>
              <li>Axios</li>
              <li>Sass</li>
              <li>Quill</li>
              <li>...</li>
            </ul>
          </el-col>
        </el-row>
      </el-col>
    </el-row>
    <el-divider />
    <el-row :gutter="20">
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <template v-slot:header>
            <div class="clearfix">
              <span>更新日志</span>
            </div>
          </template>
          <el-collapse accordion>
            <el-collapse-item title="v1.0.0 - 2025-10-1">
              <ol>
                <li>东洲科技后台管理ERP系统正式发布</li>
              </ol>
            </el-collapse-item>
          </el-collapse>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script setup name="Index">
const version = ref('1.0.0')

function goTarget(url) {
  window.open(url, '__blank')
}
</script>

<style scoped lang="scss">
.home {
  blockquote {
    padding: 10px 20px;
    margin: 0 0 20px;
    font-size: 17.5px;
    border-left: 5px solid #eee;
  }

  hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid #eee;
  }

  .col-item {
    margin-bottom: 20px;
  }

  ul {
    padding: 0;
    margin: 0;
  }

  font-family: "open sans",
  "Helvetica Neue",
  Helvetica,
  Arial,
  sans-serif;
  font-size: 13px;
  color: #676a6c;
  overflow-x: hidden;

  ul {
    list-style-type: none;
  }

  h4 {
    margin-top: 0px;
  }

  h2 {
    margin-top: 10px;
    font-size: 26px;
    font-weight: 100;
  }

  p {
    margin-top: 10px;

    b {
      font-weight: 700;
    }
  }

  .update-log {
    ol {
      display: block;
      list-style-type: decimal;
      margin-block-start: 1em;
      margin-block-end: 1em;
      margin-inline-start: 0;
      margin-inline-end: 0;
      padding-inline-start: 40px;
    }
  }
}
</style>
