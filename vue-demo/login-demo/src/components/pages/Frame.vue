<template>
  <el-container>
    <el-header>
      <Header />
    </el-header>
    <el-container>
      <el-aside>
        <Aside />
      </el-aside>
      <el-main>
        <Content />
      </el-main>
    </el-container>
  </el-container>
</template>
<script>
import Header from '../common/Header.vue'
import Aside from '../common/Aside.vue'
import Content from '../common/Content.vue'
export default {
  name: 'Frame',
  components: {
    Header,
    Aside,
    Content
  }
}

</script>
<style>
li a {
  text-decoration: none;
}

.el-container {
  height: 1000px;
  margin: 0;
}

.el-header {
  margin: 0;
  padding: 0;
}

.el-aside {
  background-color: #545c64;
}

.el-aside>ul {
  width: 100%
}

</style>
