<template>
  <ul class="w-full text-gray-600 leading-snug pt-4 md:pt-0">
    <TimelineItem period title="Work Experience & Projects" when="">
    <h2>ECOMMERCE WEB APPLICATION</h2>
    <p>Technologies:React js , javascript,mysql My Role : React js , javascript Developer</p>
    <h2>BURGER BUILDER PROJECT</h2>
    <p>Technologies:React js , javascript,mysql  My Role : React js , javascript Developer</p>
    <h2>LIBRARY MANAGEMENT PROJECT</h2>
    <p>Technologies: MySQL, Xampp Server,PHP,JS,HTML,CSS My role :mysql database , frontend Developer</p>
  <h2>ONLINE BUS TICKET RESVERATION PROJECT</h2>
   <p>Technologies: javascript,php ,ajax,mysql My role: project frontend and backend</p>
       <h2>ONLINE JOB HIRING SYSTEM PROJECT</h2>
   <p>Technologies: MySQL, Xampp Server,PHP,JS,HTML,CSS  My role :Backend and database development</p>
    </TimelineItem>
  </ul>
</template>

<script>
import TimelineItem from '~/components/TimelineItem.vue'

export default {
  name: 'Projects',
  components: { TimelineItem }
}
</script>

<style lang="postcss">
  .developmint {
    color: #15831d;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
</style>
