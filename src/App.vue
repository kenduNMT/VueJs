<script setup lang="ts">
import ColorBox from './components/ColorBox.vue'
import Test from './components/Test.vue'
import ListCourse from './components/ListCourse.vue'
import Card from './components/Card.vue'
import Calculation from './components/Calculation.vue'
import UserInfo from './components/UserInfo.vue'
import FormatName from './components/FormatName.vue'
import AdminIndex from './components/AdminIndexs.vue'
import ManagerUser from './components/ManagerUsers.vue'

</script>
<template>
  <ManagerUser></ManagerUser>
  <AdminIndex />
  <FormatName />
  <UserInfo />
  <Calculation></Calculation>
  <ColorBox></ColorBox>
  <Test />
  <ListCourse></ListCourse>
  <h1>sadasd</h1>
  <Card></Card>
</template>

<style scoped lang="scss">
h1{
  color: red;
}
</style>
