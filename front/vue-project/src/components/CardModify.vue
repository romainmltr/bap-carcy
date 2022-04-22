<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>


  <template>

    <template>
      <div class="nav-right visible-xs">
        <div class="button" id="btn">
          <div class="bar top"></div>
          <div class="bar middle"></div>
          <div class="bar bottom"></div>
        </div>
      </div>
      <!-- nav-right -->
      <main>


        <nav>
          <div class="nav-right hidden-xs">
            <div class="button" id="btn">
              <div class="bar top"></div>
              <div class="bar middle"></div>
              <div class="bar bottom"></div>
            </div>
          </div>
          <!-- nav-right -->
        </nav>

      </main>

      <div class="sidebar">
        <ul class="sidebar-list">
          <li class="sidebar-item"><a href="#" class="sidebar-anchor">Item 1</a></li>
          <li class="sidebar-item"><a href="#" class="sidebar-anchor">Item 2</a></li>
          <li class="sidebar-item"><a href="#" class="sidebar-anchor">Item 3</a></li>
          <li class="sidebar-item"><a href="#" class="sidebar-anchor">Item 4</a></li>
        </ul>
      </div>
  </template>

<style lang="sass" rel="stylesheet/scss">
/* write SCSS here */

</style>
