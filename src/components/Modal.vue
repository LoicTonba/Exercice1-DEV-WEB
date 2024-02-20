<template>
   
   
    <!-- Modal 1 -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
   <div class="modal-dialog">
       <div class="modal-content">
           <div class="modal-header">
            <h1 class="modal-title fs-5" id="exampleModalLabel">Ajouter un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
       <div class="h3">Fonctionnalité non encore disponible,… fermez la fenêtre…</div>
    </div>
   <div class="modal-footer">
    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
    <button type="button" class="btn btn-primary">Save changes</button>
   </div>
</div>
</div>
</div>

<!-- Modal2 -->
<div class="modal fade" id="exampleModal1" tabindex="-1" aria-labelledby="exampleModalLabel1" aria-hidden="true">
   <div class="modal-dialog">
       <div class="modal-content">
           <div class="modal-header">
            <h1 class="modal-title fs-5" id="exampleModalLabel1">Modifier un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
       <div class="h3">Fonctionnalité non encore disponible,… fermez la fenêtre…</div>
    </div>
   <div class="modal-footer">
    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
    <button type="button" class="btn btn-primary">Save changes</button>
   </div>
</div>
</div>
</div>

<!-- Modal3 -->
<div class="modal fade" id="exampleModal2" tabindex="-1" aria-labelledby="exampleModalLabel2" aria-hidden="true">
   <div class="modal-dialog">
       <div class="modal-content">
           <div class="modal-header">
            <h1 class="modal-title fs-5" id="exampleModalLabel2">Supprimer un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
       <div class="h3">Fonctionnalité non encore disponible,… fermez la fenêtre…</div>
    </div>
   <div class="modal-footer">
    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
    <button type="button" class="btn btn-primary">Save changes</button>
   </div>
</div>
</div>
</div>

  <!-- Modal4 -->
  <div class="modal fade" id="exampleModal3" tabindex="-1" aria-labelledby="exampleModalLabel3" aria-hidden="true">
   <div class="modal-dialog">
       <div class="modal-content">
           <div class="modal-header">
            <h1 class="modal-title fs-5" id="exampleModalLabel3">Afficher un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
       <div class="h3">Fonctionnalité non encore disponible,… fermez la fenêtre…</div>
    </div>
   <div class="modal-footer">
    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
    <button type="button" class="btn btn-primary">Save changes</button>
   </div>
</div>
</div>
</div>


<!-- Modal5 -->
<div class="modal fade" id="exampleModal4" tabindex="-1" aria-labelledby="exampleModalLabel4" aria-hidden="true">
   <div class="modal-dialog modal-lg">
       <div class="modal-content">
           <div class="modal-header card-header bg-success text-white text-center">
            <h1 class="modal-title fs-5" id="exampleModalLabel4">Afficher un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
      <div class="container">
       <div class="row">
           <div class="col">
               <div class="dashboard">
                   <div >
                   <!-- the stuff on your left nav -->
                   <form action="">
                <!-- ... Ajouter le contenu du formulaire Supprimer ici ... -->
                <div>
                             <!-- <p title="Article" class="text-center font-bold">Article</p>
                              <p class="placeholder col-12 placeholder-xs"></p> -->
                              
                             <div>
                                  
                                  <label for="">N°............................</label>  
                                  <input type="number" selectedRecordset="recordset"> <br><br>  
                                  <!-- <input type="number" v-model="recordset.No_"> <br><br> -->
                                  <label for="">Description..........</label>
                                  <input type="text"> <br><br> 
                                  <!-- <input type="text" v-model="recordset.Description"><br><br>-->
                                  <label for="" >Type........................</label>
                                  <input type="text" value=""> <br><br> 
                                  <!-- <input  type="checkbox" v-model="recordset.bloque"  id="'bloque' + recordset.No_" :checked="recordset.Bloqué">  <br><br>-->
                                  <label for="">Unité de base......</label>
                                  <select name="UniteDeBase" id="">
                                  <option value="">PCS</option>
                                  <option value="">PCS2</option>
                                  </select> <br><br>
                                  <label class="form-check-label" for="flexSwitchCheckReverse">Bloqué...................</label>
                                  <input class="form-check-input" type="checkbox" id="flexSwitchCheckReverse">
                                  <!--<div class="form-check form-switch form-check-reverse">
                                      <label class="form-check-label" for="flexSwitchCheckReverse">Bloqué...................</label>
                                      <input class="form-check-input" type="checkbox" id="flexSwitchCheckReverse">
                                  </div>  -->
                                  <!-- <input  type="checkbox" v-model="recordset.bloque"  id="'bloque' + recordset.No_" :checked="recordset.Bloqué">  <br><br> -->
  
  
                              </div>
                          </div>
                          <div>
                              <!--<p title="Stock" class="text-center font-bold">Stock</p>
                              <p class="placeholder col-12 placeholder-xs mb-5"></p> -->
                              <div>
                                  <label for="">Quantité en stock..................................</label>
                                  <input type="number"> <br><br> 
                                  <!-- <input type="number" v-model="recordset.No_"><br><br> -->
                                 <label for="">Quantité sur commande d'achat.....</label>
                                  <input type="number"> <br><br> 
                                  <!-- <input type="number" v-model="recordset.No_"><br><br> -->
                             </div>
                          </div>
              </form>
                   </div>

                   <div >
                    <!-- the stuff on your right nav 
                    <p class="h3">Oh oui je suis du cote droit</p>-->
                   </div>
               </div>
           </div>
       </div>
      </div>
    </div>
</div>
</div>
</div>


<!-- Modal6 -->
<div class="modal fade" id="exampleModal5" tabindex="-1" aria-labelledby="exampleModalLabel5" aria-hidden="true">
   <div class="modal-dialog modal-lg">
       <div class="modal-content">
           <div class="modal-header card-header bg-success text-white text-center">
            <h1 class="modal-title fs-5" id="exampleModalLabel5">Modifier un article</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
    <div class="modal-body">
      <div class="container">
       <div class="row">
           <div class="col">
               <div class="dashboard">
                   <div >
                   <!-- the stuff on your left nav -->
                   <form action="">
                <!-- ... Ajouter le contenu du formulaire Supprimer ici ... -->
                <div>
                             <!-- <p title="Article" class="text-center font-bold">Article</p>
                              <p class="placeholder col-12 placeholder-xs"></p> -->
                              
                             <div>
                                  
                                  <label for="">N°............................</label>  
                                  <input type="number"> <br><br>  
                                  <!-- <input type="number" v-model="recordset.No_"> <br><br> -->
                                  <label for="">Description..........</label>
                                  <input type="text"> <br><br> 
                                  <!-- <input type="text" v-model="recordset.Description"><br><br>-->
                                  <label for="" >Type........................</label>
                                  <input type="text" value=""> <br><br> 
                                  <!-- <input  type="checkbox" v-model="recordset.bloque"  id="'bloque' + recordset.No_" :checked="recordset.Bloqué">  <br><br>-->
                                  <label for="">Unité de base......</label>
                                  <select name="UniteDeBase" id="">
                                  <option value="">PCS</option>
                                  <option value="">PCS2</option>
                                  </select> <br><br>
                                  <label class="form-check-label" for="flexSwitchCheckReverse">Bloqué...................</label>
                                  <input class="form-check-input" type="checkbox" id="flexSwitchCheckReverse">
                                  <!--<div class="form-check form-switch form-check-reverse">
                                      <label class="form-check-label" for="flexSwitchCheckReverse">Bloqué...................</label>
                                      <input class="form-check-input" type="checkbox" id="flexSwitchCheckReverse">
                                  </div>  -->
                                  <!-- <input  type="checkbox" v-model="recordset.bloque"  id="'bloque' + recordset.No_" :checked="recordset.Bloqué">  <br><br> -->
  
  
                              </div>
                          </div>
                          <div>
                              <!--<p title="Stock" class="text-center font-bold">Stock</p>
                              <p class="placeholder col-12 placeholder-xs mb-5"></p> -->
                              <div>
                                  <label for="">Quantité en stock..................................</label>
                                  <input type="number"> <br><br> 
                                  <!-- <input type="number" v-model="recordset.No_"><br><br> -->
                                 <label for="">Quantité sur commande d'achat.....</label>
                                  <input type="number"> <br><br> 
                                  <!-- <input type="number" v-model="recordset.No_"><br><br> -->
                             </div>
                          </div>
              </form>
                   </div>

                   <div >
                    <!-- the stuff on your right nav -->
                    <!--<p class="h3">Oh oui je suis du cote droit</p> -->
                   </div>
               </div>
           </div>
       </div>
      </div>
    </div>
</div>
</div>
</div>

</template>


<script>
    import axios from "axios";
    export default {
    name: "Mo_dal",
    data() {
        return {
            showModal : false,
            recordsets: [],
            selectedRecordset: {},
        };
    },

    mounted() {
        axios.get("http://localhost:3000/app").then((response) => {
        this.recordsets = response.data.recordsets[0];
    });
    },
};
</script>

<style scoped>
    .dashboard{
        width: 100vw;
    }
  
    
</style>