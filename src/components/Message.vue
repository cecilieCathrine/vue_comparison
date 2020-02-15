<template>
    <span>{{message}}</span>
</template>

<script>
export default {
  name: "Message",
   props: {
    message: {
      type: String
    },
  },

};
</script>
