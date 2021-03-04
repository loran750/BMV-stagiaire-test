<template>
  <div id="app">
    <h1>Exercice VueJS</h1>

    <p>
      La variable form ci-dessous contient un flux json représentant un formulaire web. Il est constitué : 
      <ul>
        <li>De deux input text</li>
        <li>Un champ select</li>
        <li>Un champ checkbox</li>
      </ul>      
    </p>
    <div style="padding:15px">
      <h2>Exercice 1</h2>
      <p>Afficher en html les deux input qui sont de type texte</p>

      <h2>Exercice 2</h2>
      <p>Afficher en html le champ select. Faire de même ensuite avec le champ checkbox</p>

      <h2>Exercice 3</h2>
      <p>Remplir les variables input1, input2, optionSelected et checkedItem avec ce qui a été saisi par l'utilisateur coté front</p>
    </div>
    <h3>Illustration du résultat attendu :</h3> 
    <img alt="Vue logo" src="./assets/resultat.png">
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
    
  },  
  data: function () {
    return { 
        input1:'',
        input2:'',
        optionSelected:'',
        checkedItem:'',
        form: {"attributes":[{"id":3,"key":"9eb6b76f-2f67-4b49-8c9e-8d39d563c80d","label":"Description","instructions":"ne doit pas s'afficher","input":"text","type":"description","required":1,"hidden":0,"default":null,"priority":2,"options":"[]","cardinality":0,"config":"[]","response_private":0,"description":null,"show_checkbox":0},{"id":4,"key":"5d1cbb88-dc6f-4a6d-a1e5-f3c0c38e132b","label":"Title","instructions":null,"input":"text","type":"title","required":1,"hidden":0,"default":null,"priority":1,"options":"[]","cardinality":0,"config":"[]","response_private":0,"description":null,"show_checkbox":0},{"id":156,"key":"96f0a1c2-94e3-40d5-8a16-c38ca0bd19c2","label":"Ma select","instructions":null,"input":"select","type":"varchar","required":0,"hidden":0,"default":null,"priority":9,"options":"[\"Laurent\",\"Samuel\",\"Claire\"]","cardinality":1,"config":"[]","response_private":0,"description":null,"show_checkbox":0},{"id":157,"key":"83b9cd4a-0ac1-493c-a797-ae8df5998f0d","label":"Combien ?","instructions":null,"input":"checkbox","type":"varchar","required":0,"hidden":0,"default":null,"priority":10,"options":"[\"Rien\",\"Tout\",\"42\",\"Chat\\\/20\"]","cardinality":0,"config":"[]","response_private":0,"description":null,"show_checkbox":0}]}
    
    }
  },
}
</script>