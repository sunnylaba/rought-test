<template>
<button type="button" class="btn btn-primary" @click="getRoute">getRoute</button>

<button type="button" class="btn btn-primary" @click="push">push</button>
<button type="button" class="btn btn-primary" @click="replace">replace</button>
<button type="button" class="btn btn-primary" @click="go">go</button>
<hr />
<button type="button" class="btn btn-primary" @click="addRoute">新增路由</button>
</template>

<script>
export default {
  methods: {
    getRoute() {
    // 取得路由的屬性
    // console.log(this.$route);

      // 呼叫路由的方法
      console.log(this.$router);
    },
    push() {
      this.$router.push({
        name: 'About',
      });
    },
    // 沒有歷史紀錄
    replace() {
      this.$router.replace({
        name: 'About',
      });
    },
    // 操作歷史紀錄
    go() {
      this.$router.go(-1);
    },
  },
};
</script>
