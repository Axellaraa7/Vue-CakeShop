<template>
  <PedidosComponent/>
</template>

<script>
import PedidosComponent from "../components/PedidosComponent.vue";
export default {
  name: "AdminPedidosView",
  components:{
    PedidosComponent
  },
  created(){
    this.changeUser();
  },
  methods:{
    changeUser(){
      this.$store.dispatch("changeUser",true);
    }
  }
}
</script>