  <template>
    <div class="formulaire">
        <h1>Formulaire</h1>
        <div>

          <!-- <div>
            <h2>Compétence</h2>
            <p>Nom de la Compétence</p>
            <input v-model="nomCompetence" />
            <br>
            <p>Date de début</p>
            <input v-model="dateDebutCompetence" />
            <br>
            <p>Date de fin</p>
            <input v-model="dateFinCompetence" />
            <br>
            <button @click="saveEnregistrer">Enregistrer</button>
          </div>

         <div>
            <h2>Divers</h2>
            <p>Nom de l'activité</p>
            <input v-model="nomActivite" />
            <br>
            <p>Date de début</p>
            <input v-model="dateDebutActivite" />
            <br>
            <p>Date de fin</p>
            <input v-model="dateFinActivite" />
            <br>
            <button @click="saveEnregistrer">Enregistrer</button>
          </div>

          <div>
            <h2>Expérience</h2>
            <p>Nom de l'expérience</p>
            <input v-model="nomExperience" />
            <br>
            <p>Date de début</p>
            <input v-model="dateDebutExperience" />
            <br>
            <p>Date de fin</p>
            <input v-model="dateFinExperience" />
            <br>
            <button @click="saveEnregistrer">Enregistrer</button>
          </div> -->

          <div>
            <h2>Formation</h2>
            <p>Nom de la formation</p>
            <input v-model="nomFormation" />
            <br>
            <!-- <p>Date de début</p>
            <input v-model="dateDebutFormation" />
            <br>
            <p>Date de fin</p>
            <input v-model="dateFinFormation" />
            <br> -->
            <button @click="saveFormation">Enregistrer</button>
          </div>
          <thead>
              <tr>
                  <th>Nom de la formation</th>
                  <!-- <th>début de la formation</th>
                  <th>fin de la formation</th> -->
              </tr>
          </thead>
          <tbody>
              <!-- https://v2.vuejs.org/v2/guide/list.html -->
            <tr v-for="formationTab in formationTabs" :key="formationTab.saveFormation">
                <td>{{formationTab.nomFormation}}</td>
                <!-- <td>{{formationTab.dateDebutFormation}}</td>
                <td>{{formationTab.dateFinFormation}}</td> -->
            </tr>
          </tbody>
        </div>
    </div>
  </template>

  <script>
    export default {
        name: 'formulaireFormation',
        data: function() {
            return {
            formationTabs: ""
            }
        },

        methods: {
        saveFormation: function (message) {
        this.nomFormation = (message)
        alert("vous avez une nouvelle formation:" + this.nomFormation)
    }
        }
        }

</script>

  <style>
  </style>
  