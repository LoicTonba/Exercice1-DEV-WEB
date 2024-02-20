<template>
    <Navbar/>
    <Modal/>
   <div class="container mt-3">
    <div class="d-grid gap-2 d-md-block text-center">
                <!-- Button trigger modal Ajouter -->
                <button type="button" class="btn btn-primary m-4" data-bs-toggle="modal" data-bs-target="#exampleModal">
                     Ajouter
                </button>

         
           <!-- Button trigger modal Supprimer-->
                <button type="button" class="btn btn-primary m-4" data-bs-toggle="modal" data-bs-target="#exampleModal1">
                     Modifier
                </button>

            
      

          <!-- Button trigger modal Modifier -->
                <button type="button" class="btn btn-primary m-4" data-bs-toggle="modal" data-bs-target="#exampleModal2">
                     Supprimer
                </button>

                
    
      <!-- Button trigger modal Afficher -->
      <button type="button" class="btn btn-primary m-4" data-bs-toggle="modal" data-bs-target="#exampleModal3">
                     Afficher
                </button>
             
    </div>
 </div>
    
     <div class="card shadow-lg">
        <div class="container w-95 pt-5">
        <table id="example" class="table table-striped w-100">
          <thead class="table-primary">
            <tr>
              <th>No_</th>
              <th>Description</th>
              <th>Type</th>
              <th>Unité de Base</th>
              <th>Image</th>
              <th>Quantité en Stock</th>
              <th>Quantité sur commande d'achat</th>
              <th>Bloqué</th>
              <th>Actions</th>
            </tr>
          </thead>
          <tbody>
            <tr class="recordsetsItemContainer" v-for="recordset in recordsets" :key="recordset.No_">
              <td>{{ recordset.No_ }}</td>
              <td>{{ recordset.Description }}</td>
              <td>{{ recordset.Type==0? "Stock": recordset.Type==1? "Service": "Hors Stock"}}</td>
              <td>{{ recordset["Unité de Base"] }}</td>
              <td>{{recordset.Image}}</td>
              <td>{{ recordset["Quantité en Stock"] }}</td>
              <td>{{ recordset["Quantité sur commande d'achat"] }}</td>
              <td> <input  type="checkbox" v-model="recordset.bloque"  id="'bloque' + recordset.No_" :checked="recordset.Bloqué"> </td>
               <!-- Button trigger modal Afficher -->
               <button type="button" class="btn btn-success btn-sm m-1 shadow-lg" data-bs-toggle="modal" data-bs-target="#exampleModal4">
                     Afficher
                </button>
               <!-- Button trigger modal Afficher -->
                 <button type="button" class="btn btn-warning btn-sm m-1 shadow-lg" data-bs-toggle="modal" data-bs-target="#exampleModal5">
                     Modifier
                 </button>
            </tr>
          </tbody>
          <tfoot>
          <div>
            <tr>
            <td colspan="8">
              <!--<p>Lignes : {{ recordsets.length }}</p> -->
              <p class="ligne">Total de lignes : {{ recordsets.length }}</p>
            </td>
          </tr>
          </div>
        </tfoot>
          
        </table>
      </div>
     </div>
    </template>
    
    <script>
    import axios from "axios";
    
   
    export default {
      name: "record_sets",
    
      data() {
        return {
          recordsets: [],
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
/* Pas besoin de définir le style pour d-grid, gap-2, d-md-block ici car ils sont utilisés dans le template seulement */

/* Style pour le centrage des boutons */
.d-grid.text-center {
  margin-left: 20px;
}

/* Style pour centrer la table */
.container.pt-5 {
  text-align: center;
}

/* Ajout de la marge en bas à tous les boutons sauf le dernier */
.btn btn-primary {
  margin-bottom: 20px;
}

.card shadow-lg{
    bs-table-border-color: var(--bs-border-color);
}

/*.ligne{
    margin-right: 30px;
} */
</style>