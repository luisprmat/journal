<template>
  <div
    class="entry-container mb-3 p-2 pointer"
    @click="$router.push({ name: 'entry', params: { id: 10 } })"
  >

    <!-- Titulo -->
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">23</span>
      <span class="mx-1 fs-5">Febrero</span>
      <span class="mx-1 fw-light">2022, miércoles</span>
    </div>

    <div class="entry-description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed fuga velit deserunt architecto mollitia fugit officia. Dicta et quidem architecto aut quas reprehenderit consequuntur accusantium temporibus, sint voluptates, quaerat nam?
    </div>
  </div>
</template>

<style lang="scss" scoped>
.entry-container {
  border-bottom: 1px solid #2c3e50;
  transition: 0.2s all ease-in;

  &:hover {
    background-color: lighten($color: gray, $amount: 45);
    transition: 0.2s all ease-in;
  }

  .entry-description {
    font-size: 12px;
  }
}
</style>
