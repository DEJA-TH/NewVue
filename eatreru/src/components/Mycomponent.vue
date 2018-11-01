<template>
  <button @click="myfunc(font)">{{font}}</button>
</template>

<script>
  export default {
    props : {
      font : {
        type : String
      },
      myfunc : {
        type : Function
      },
      data () {
        return {
          text : "Message"
        }
      }
    }
  }
</script>
