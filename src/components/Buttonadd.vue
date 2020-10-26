<template>
    <div id="btn" class="btns">
      <!-- <el-button class="btnstyle" @click="show(n)"  :key="n" v-for="n in nums" type="info">{{n}}</el-button> -->
      <div class="btnstyle"  :key="n" v-for="n in nums" type="info"> <el-button class="btnstyle" @click="show(n)"   type="info">{{n}}</el-button></div>
    </div>
</template>
<script >
export default {
  data () {
    return {
      nums: [
        1, 2, 3, 4, 5
      ]
    }
  },
  methods: {
    show (n) {
      console.log(n)
      // alert()
    }
  }
}

</script>
<style scoped>
 .btns {
    margin: 0 auto;
    width: 90%;
    display: flex;
    flex-flow: row wrap;
}
.btnstyle {
  flex: 0 0 30%;
  margin: 5px;
  text-align: center;
}
.el-button {
  width: 180px;
  height: 30px;
}
</style>
