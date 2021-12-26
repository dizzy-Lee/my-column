<template>
  <column-list :list="list"></column-list>
</template>

<script lang="ts">
import "bootstrap/dist/css/bootstrap.min.css";
import { defineComponent } from "vue";
import ColumnList, { ColumnProps } from "./components/ColumnList.vue";
const ColumnListTestData: ColumnProps[] = [
  {
    id: 0o1,
    title: "my column 1",
    description: "this is a description",
    avatar: "https://img2.baidu.com/it/u=1520747491,3988420976&fm=26&fmt=auto",
  },
  {
    id: 0o2,
    title: "my column 2",
    description: "this is a description",
    avatar: "https://img2.baidu.com/it/u=1520747491,3988420976&fm=26&fmt=auto",
  },
  {
    id: 0o3,
    title: "my column 3",
    description: "this is a description",
  },
  {
    id: 0o2,
    title: "my column 2",
    description: "this is a description",
    avatar: "https://img2.baidu.com/it/u=1520747491,3988420976&fm=26&fmt=auto",
  },
];
export default defineComponent({
  name: "App",
  components: {
    ColumnList,
  },
  setup() {
    return {
      list: ColumnListTestData,
    };
  },
});
</script>

<style></style>
