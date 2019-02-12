<template>
  <div>
    <form @submit="addTodo">
      <div class="todoForm" style="display: flex">
        <div style="flex: 1 0 auto">
          <input class="textInput" type="text" v-model="title" name="title" placeholder="add todo">
        </div>
        <div style="flex: 0 1 auto">
          <input type="submit" value="Submit" class="btn">
        </div>
      </div>
    </form>
  </div>
</template>
<script>
export default {
  name: "AddTodo",
  data() {
    return {
      title: ""
    };
  },
  methods: {
    addTodo(e) {
      e.preventDefault();
      const newTodo = {
        title: this.title,
        complete: false
      };
      this.$emit("add-todo", newTodo);
      this.title = "";
    }
  }
};
</script>
<style scoped>
.todoForm {
  width: 100%;
}
.textInput {
  width: 100%;
}
</style>


