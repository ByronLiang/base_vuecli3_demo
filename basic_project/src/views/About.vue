<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'about',
  components: {
    
  },
  data() {
      return {
          form: {
              content: '',
              content2: '',
          },
      };
  },
  methods: {
    fetch() {
      API.get('type').then((r) => {
        console.log(r);
      });
    }
  },
  mounted() {
    console.log('abc');
    this.fetch();
  },
}
</script>
