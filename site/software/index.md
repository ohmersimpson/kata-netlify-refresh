---
title: Software
subhead: Development activities in Kata Containers
description: Development activities in Kata Containers
---

Kata Containers is Apache 2 licensed software consisting of six components: Agent, Runtime, Proxy, Shim, Kernel and packaging of QEMU 2.11. It is designed to be architecture agnostic, run on multiple hypervisors and plug seamlessly into the containers ecosystem.
<br>

<a href="#" class="button is-primary-dark is-rounded">
  <span>EXPLORE ON GITHUB</span>

  <span class="ico">
    <img src="../.vuepress/theme/svg/arrow-left.svg" alt="Learn More" />
  </span>
</a>

<br>
<br>


## Architecture

  <a href="/images/Airship_Diagram_SimplifiedArchitecture.jpg">
    <img
      src="/images/Airship_Diagram_SimplifiedArchitecture.jpg"
      alt="title"
    />
  </a>


<br>

<div class="columns">
  <div class="column">
    <div class="box is-green">
     <div class="box-text"><div class="software-icon"><figure class="image is-64x64">
      <img src="../.vuepress/theme/svg/logo_ico1.svg">
      </figure></div><h3 class="is-software">Get Kata Containers</h3>
      <a href="https://git.katacontainers.io/cgit" class="a-primary-blue" >
        Go to Git Repository &nbsp <img src="../.vuepress/theme/svg/arrow-left_primary-dark.svg" class="a-primary-blue">
      </a></div>
    </div>
  </div>
  <div class="column">
    <div class="box is-green">
     <div class="box-text"><div class="software-icon" style="align-content: middle"><figure class="image is-64x64">
      <img style="height: 56.13px" src="../.vuepress/theme/svg/document_primary-dark.svg">
      </figure></div><h3 class="is-software">View the Documentation</h3>
      <a href="https://airship-treasuremap.readthedocs.io/en/latest/" class="a-primary-blue">
        Get Started &nbsp <img src="../.vuepress/theme/svg/arrow-left_primary-dark.svg">
      </a></div>
    </div>
  </div>
</div>

<br>



## Kata Containers Integration with Kubernets:

  <a href="/images/Airship_Diagram_SimplifiedArchitecture.jpg">
    <img
      src="/images/Airship_Diagram_SimplifiedArchitecture.jpg"
      alt="title"
    />
  </a>

<!-- ## Kata Containers Integration with Kubernets:
### Kata Containers Integration with Kubernets:
#### Kata Containers Integration with Kubernets:
##### Kata Containers Integration with Kubernets: -->


<div class="container1">
  <h2 class="features">Integration Points</h2>
</div>


<div class="container2">

<div class="columns">

  <div class="column col1">
  
  <h4 class='is-centered'>Hypervisor:</h4>
    <span>Firecracker</span>
    <span>QEMU</span>
    <span>NEMU</span>
  </div>
  
  <div class="column">
    <h4>Architecture support:</h4>
    <span>X86_64</span>
    <span>arch64</span>
    <span>ppc64le</span>
    <span>s390x</span>
  </div>

  <div class="column col3">
    <h4>Hardware support:</h4>
    <span>Nvidia GPU</span>
    <span>FPGA</span>
    <span>QAT</span>
    <span>RDMA</span>
    <span>SRIO-V</span>
  </div>

</div>

</div>


## Requirements

Kata requires nested virtualization or bare metal. The Kata Containers runtime has a built-in command (kata-check) to determine if your host system is capable of running a Kata Container. [Learn how to use kata-check]().



<div class="columns">

  <div class="column ">

  <box withActions title="Distributions">
    Kata Containers is available on many distributions. View the [distro specific install guides] () for:

  <br/>

  <div class="columns">
    <div class="column"> 
      <ul><li>CentOS</li><li>Debian</li><li>Fedora</li><li>OpenSuse</li></ul>
    </div>
    <div class="column">
      <ul><li>RHEL</li><li>SLES</li><li>Ubuntu</li></ul>
    </div>
  </div>

  </box>


  </div>
  
  <div class="column">
    
  <box withActions title="Cloud Service Platform">
    Run Kata Containers on a cloud service platform:

  <div class="columns">
  <div class="column">
    <a href="#" >Amazon Web Services</a><br/>
    <a href="#" >Microsoft Azure</a><br/>
    <a href="#" >Google Compute Engine</a><br/>
    <a href="#" >Vexxhost OpenStack Cloud</a><br/><br/><br/>
  </div>
  </div>

  </box>

  </div>

</div>