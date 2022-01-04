<template>
  <form class="container" @submit.prevent="Guardar()">
      <Form :dato="datos" />
  </form>
  <hr>
  {{this.datos}}
</template>

<script>
import Form from '../components/Inputs.vue'
export default {
    components:{
        Form
    },
    data() {
        return {
            datos:{
                id:'',
                nombre: '',
                tipo: [],
                preoridad: '',
                numero: 0
            }
        }
    },
    methods: {
        Guardar(){
            if(this.datos.nombre.trim() === ""){
                console.log("Campo Vacio");
                return;
            }   
            console.log(this.datos);
            this.datos = {
                id:'',
                nombre: '',
                tipo: [],
                preoridad: '',
                numero: 0
            }
        },  
    }

}
</script>