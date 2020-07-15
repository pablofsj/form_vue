<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12">
        <img src="https://course_report_production.s3.amazonaws.com/rich/rich_files/rich_files/2470/s300/cd-logo-blue-600x600.png" alt="" srcset="">
        <br><br><br> 
        <h1>Encuesta del Dojo</h1>
        <br><br>
      </div>
    </div>
    <div class="row">
      <div class="form-group col-sm-12">
        <label for="">Nombre</label>
        <input type="text" class="form-control" placeholder="Ingresa tu nombre completo" v-model="nombre">
      </div>
      <div class="form-group col-sm-12">
        <label for="">Ubicación de tu Dojo</label>
        <select class="form-control" v-model="ubicacion">
          <option value="" disabled selected>Elige ubicación</option>
          <option value="1">Chicago</option>
          <option value="2">Valparaíso</option>
          <option value="3">Nueva York</option>
          <option value="4">Londres</option>
        </select>
      </div>
      <div class="form-group col-sm-12">
        <label for="">Lenguaje Preferido</label>
        <select class="form-control" v-model="lenguaje">
          <option value="" disabled selected>Elige lenguaje</option>
          <option value="1">C#</option>
          <option value="2">Javascript</option>
          <option value="3">Python</option>
          <option value="4">PHP</option>
          <option value="5">Ruby</option>
          <option value="6">C++</option>
        </select>
      </div>
      <div class="form-group col-sm-12">
        <label for="">Comentarios</label>
        <textarea class="form-control" rows="3" placeholder="Déjanos acá tus comentarios" v-model="comentario"></textarea>
      </div>
      <div class="col-sm-12">
        <button type="button" class="btn btn-outline-info">Enviar</button>
        <br><br><br>
      </div>
    </div>
  </div>
</template>




<script>
export default {
  name:'Form',
  data:function() {
    return {
      nombre: '',
      ubicacion: '',
      lenguaje: '',
      comentario: ''
    };
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h1{
  color: #5dbcd2;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
