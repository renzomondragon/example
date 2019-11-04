<template>
  <div>
    <v-content>
    
        <v-parallax src="../assets/bg-circuits.png" height="720">
          <v-layout
            column
            align-center
            justify-center
          >
        <v-container class="col-md-8">
          <v-row>
            <v-col>
                <v-btn
                class="mt-12"
                color=""
                large
                @click="cambiardiv()"
              >
                Persona Natural
              </v-btn>
            </v-col>
            <v-col>
                <v-btn
                class="mt-12"
                color=""
                large
                @click="cambiardiv2()"
              >
                Empresa
              </v-btn>
            </v-col>
          </v-row>
          <v-row>
            <Form1 v-if="formulario==false"/> 
            <Form2 v-if="formulario==true"/>
          </v-row>
        </v-container>
        <v-row>
            <v-col>
            <v-btn
            class="mt-25"
            color="dark"
            dark
            large
            href=""
          >
            OBTENER DESCUENTO
          </v-btn>
          </v-col>  
        </v-row>
          </v-layout>
        </v-parallax>
 
    </v-content>
    </div>
</template>



<script>
import Form1 from './form1'
import Form2 from './form2'
export default {
  components:{
    Form1,
    Form2
  },
  
  data: () => ({
    formulario: false,
    //
  }),
  methods:{
    cambiardiv(){
        let dato = true
        this.formulario=dato     
    },
    cambiardiv2(){
       let dato = false
        this.formulario=dato   
    }
}
}
</script>