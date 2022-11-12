<template>
  <div class="home">
    <div class="home_Nav">
      <el-row class="home_Nav_row">
        <el-col :span="3" v-for="(arr, index) in navBar" :key="index">
          <div>
            <a :href="arr.path">{{ arr.name }}</a>
          </div>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
import { reactive } from "vue";
export default {
  name: "hoME",
  setup() {
    const navBar = reactive([
      { name: "点击去我的csdn", path: "https://www.csdn.net/" },
      { name: "点击去我查看源码", path: "https://www.csdn.net/" },
      { name: "点击去我的掘金", path: "https://www.csdn.net/" },
      { name: "待开发项目", path: "https://www.csdn.net/" },
      { name: "待开发项目", path: "https://www.csdn.net/" },
      { name: "待开发项目", path: "https://www.csdn.net/" },
      { name: "待开发项目", path: "https://www.csdn.net/" },
      { name: "待开发项目", path: "https://www.csdn.net/" },
    ]);
    return {
      navBar,
    };
  },
};
</script>

<style scope>
.home_Nav_row {
  height: 10vh;
  line-height: 10vh;
  text-align: center;
}
</style>
