<template>
  <main class="main">
    <hero class="hero-main is-primary" withButton :title="$page.frontmatter.hero.headline" :image="require('../theme/images/hero-image.png')">
      <template slot="buttons">
        <a :href="$page.frontmatter.hero.button.url" class="button is-primary-dark is-rounded">
          <span>{{ $page.frontmatter.hero.button.title }}</span>

          <span class="ico">
            <img :src="require('../theme/svg/arrow-left.svg')" alt="Learn More" />
          </span>
        </a>
      </template>
    </hero>

    <base-article :image="require('../theme/images/kata-explained1@2x.png')">
      <slot name="about"></slot>
    </base-article>
<!-- Features Table -->    
<div class="features-section">
<div class="container">
  <h2 class="features">Features</h2>
  <table class="table" style="width:100%; background-color: white;">
    <tbody>
      <tr>
        <td class="is-selected is-primary-blue"><img class="feature-icons" :src="require('../theme/svg/security-badge.svg')" alt="Security"/><h6>Security</h6></td>
        <td>Runs in a dedicated kernel, providing isolation of network, I/O and memory and can utilize hardware-enforced isolation with virtualization VT extensions.</td>
      </tr>
      <tr>
        <td class="is-selected is-primary-blue"><img class="feature-icons" :src="require('../theme/svg/compatibiity-badge.svg')" alt="Compatibility"/><h6>Compatibility</h6></td>
        <td>Supports industry standards including OCI container format, Kubernetes CRI interface, as well as legacy virtualization technologies.</td>
      </tr>
      <tr>
        <td class="is-selected is-primary-blue"><img class="feature-icons" :src="require('../theme/svg/preformance-growth.svg')" alt="Performance"/><h6>Performance</h6></td>
        <td>Delivers consistent performance as standard Linux containers; increased isolation with the performance tax of standard virtual machines.</td>
      </tr>
      <tr>
        <td class="is-selected is-primary-blue"><img class="feature-icons" :src="require('../theme/svg/bullseye-simplicity.svg')" alt="Simplicity"/><h6>Simplicity</h6></td>
        <td>Eliminates the requirement for nesting containers inside full blown virtual machines; standard interfaces make it easy to plug in and get started.</td>
      </tr>
    </tbody>
  </table>
</div>  
</div>
<!-- /Features Table -->
    <base-section class="section-modified">
      <div class="section-inner">
        <div class="columns">
          <div class="column">
            <list-numeric title="How to Get Involved" :items="$page.frontmatter.getInvolvedSteps">
              <template slot-scope="{ item }">
                <h6>{{ item.title }}</h6>

                <p>{{ item.entry }}</p>

                <a :href="item.link.url">{{ item.link.title }}</a>
              </template>
            </list-numeric>
          </div><!-- /.column -->

          <div class="column">
            <slot name="announcement"></slot>
          </div><!-- /.column -->
        </div><!-- /.columns -->
      </div><!-- /.section-inner -->
    </base-section>


 <section class="section search-content">

  <div class="search-content">
    <h3 class="search-content-title">Are your running Kata Containers? frank</h3>
    <!-- /.hero-title -->
    <div class="search-content-subtitle">Stay up to date on Kata Containers and Open Infrastructure community news.
    </div>
    <div v-if="withEntry" class="hero-entry">
      <slot name="entry"/>
    </div>
    <!-- /.hero-entry -->
    <div v-if="withButton" class="hero-actions">
      <slot name="buttons"/>
    </div>
    <!-- /.hero-actions -->
  </div>

  <b-field position="is-centered">
    <input placeholder="Email Address" type="input" class="search-container-input" size="is-large">
    </input>
    <p class="control">
      <!-- <button class="search-container-submit">Search</button> -->
      <a :href="link" class="button is-primary no-border-radius">
        <span>SUBMIT</span>
        
        <span class="ico">
          <img :src="require('../theme/svg/arrow-left.svg')" alt="Call To Action">
        </span>
      </a>
    </p>
  </b-field>



  </section>


  </main><!-- /.main -->
</template>

<script>
export default {
  /**
   * The name of the component.
   *
   * @type {Strng}
   */
  name: "SupportContact"
};
</script>