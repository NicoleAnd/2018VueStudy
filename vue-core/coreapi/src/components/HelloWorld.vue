<template>
  <div class="com">
      <mycomponent></mycomponent>
  </div>
</template>

<script>
var child = {
  template: '<div>this is my demo</div>'
}
export default {
  name: 'com',
  components: {
      'mycomponent':child
  },
  data() { 
    return {
        message:'success data'
    }
  }
 }
</script>
