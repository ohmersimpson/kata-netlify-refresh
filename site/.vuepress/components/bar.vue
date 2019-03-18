<template>
  <div class="bar is-dark-gray">
    <div class="container">
      <div class="bar-inner">
        <div class="bar-logo">
          <img :src="require('../theme/images/bar-logo.svg')" alt="Meet the Airship Community">
        </div>
        <!-- /.bar-logo -->
        <div class="bar-entry">
          <p>Meet the Kata Containers Community at the Open Infrastructure Summit, April 29–May 1, 2019 in Denver, Colorado!</p>
        </div>
        <!-- /.bar-entry -->
        <a href="//openstack.org/summit/denver-2019/" target="_blank" class="bar-btn">Learn More</a>
      </div>
      <!-- /.bar-inner -->
    </div>
    <!-- /.container -->
  </div>
  <!-- /.bar -->
</template>

<script>
export default {
  /**
   * The name of the component.
   *
   * @type {Strng}
   */
  name: "Bar"
};
</script>
