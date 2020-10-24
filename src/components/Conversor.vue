<template>
  <div class="hello">
        <div class="col-sm-12 ">
            <div class="card ">
                <div class="card-header">
                    {{nome_moeda1}} / {{nome_moeda2}}
                </div>
                <div class="card-body">
                    <label for="">{{nome_moeda1}}:</label>
                    <input v-model="value"  type="number" class="form-control">
                    <label for="">{{nome_moeda2}}:</label>
                    <input disabled v-bind:value="valor_moeda2"   type="number" class="form-control">
                    <h1 class="text-center">{{multipliedValue}}</h1>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
  name: 'Conversor',
  props: {
    nome_moeda1:String,
    nome_moeda2:String,
    valor_moeda2:Number
    
  },
  data:function(){
      return{
          value:1,
        //   valor_moeda2,
      }
  },
  computed:{
        multipliedValue () {
        console.log (this.valor_moeda2);
        return (this.value * this.valor_moeda2);
   }
  },
  methods:{
    //   converte(valor_moeda1 , valor_moeda2){
    //     //   const convertido = (parseFloat(valor_moeda) * parseFloat(valor_moeda2));
    //     //   this.valor_moeda.push(convertido);
          
    //   },
  }
}
</script>

<style scoped>
button{
    margin-top: 10px;
}
</style>
