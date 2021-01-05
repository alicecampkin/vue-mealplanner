<template>
  <section class="planner-wrapper">
    <div class="tabs">
      <div class="tabs__tab">
        <a href="#">Breakfast</a>
      </div>
      <div class="tabs__tab">
        <a href="#">Lunch</a>
      </div>
      <div class="tabs__tab">
        <a href="#">Dinner</a>
      </div>
    </div>
    <section class="planner-body">
      <slot />
      <div class="controls"></div>
    </section>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.planner-wrapper {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;

  .tabs__tab {
    background: white;
  }
}

.planner-body {
  width: 100%;
  height: 100%;
  background: white;
  border: 1px solid #ddd;
}

.controls {
  display: flex;
  justify-content: space-between;
  width: 100%;
  height: 40px;
}
</style>