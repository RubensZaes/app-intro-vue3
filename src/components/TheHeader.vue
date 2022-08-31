<template>
  <!-- <header class="header">Header</header> -->
  <div>
    <div v-for="(obj, index) in toDos" :key="obj.id" class="toDos-item">
      {{ index }} - {{ obj.title }}
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      toDos: [
        {
          userId: 1,
          id: 1,
          title: "delectus aut autem",
          completed: false,
        },
        {
          userId: 1,
          id: 2,
          title: "quis ut nam facilis et officia qui",
          completed: false,
        },
        {
          userId: 1,
          id: 3,
          title: "fugiat veniam minus",
          completed: false,
        },
        {
          userId: 1,
          id: 4,
          title: "et porro tempora",
          completed: true,
        },
        {
          userId: 1,
          id: 5,
          title:
            "laboriosam mollitia et enim quasi adipisci quia provident illum",
          completed: false,
        },
      ],
    };
  },
};
</script>

<style>
.toDos-item {
    background: #000;
    margin: 0 0 5px 0;
    padding: 3px 6px;
    color: #fff;
}
.header {
  background-color: #000;
  color: #fff;
}
</style>