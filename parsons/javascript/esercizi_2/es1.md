---
layout: default
title: JavaScript - Esercizio gruppo 2 n. 1
description: Dichiarare una variabile chiamata "numero" e assegnarle il valore 5. Mostrare il valore della variabile.
---

<div id="js_esgroup2_1-sortableTrash" class="sortable-code"></div>
<div id="js_esgroup2_1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>

<!-- Controlli per scegliere il valore -->
<label for="js_esgroup2_1-valueInput">Valore per <code>numero</code>:</label>
<input id="js_esgroup2_1-valueInput" type="text" placeholder="es. 5 oppure Ciao" />
<select id="js_esgroup2_1-valueType">
  <option value="number">Number</option>
  <option value="string">String</option>
</select>
<button id="js_esgroup2_1-setValue">Set Value &amp; (Re)create Problem</button>

<p style="margin-top:10px">
    <input id="js_esgroup2_1-feedbackLink" value="Get Feedback" type="button" />
    <input id="js_esgroup2_1-newInstanceLink" value="Reset Problem" type="button" />
</p>

<script type="text/javascript">
(function(){
  // template con placeholder VALUE (verrà sostituito)
  var template = "let numero = VALUE;\n" +
                 "console.log(numero);\n" +
                 "let nome = \"Mario\"; // distractor";

  var parsonsPuzzle = null;

  // funzione che crea (o ricrea) il widget con il valore scelto
  function createWidget(rawValue, type) {
    var valueText = rawValue;
    var variableCheckValue;

    if (type === 'string') {
      // Per le stringhe, aggiungiamo automaticamente le virgolette nel codice
      // (se l'utente ha già messo virgolette le rispettiamo)
      if (!(/^["'].*["']$/).test(rawValue)) {
        valueText = '"' + rawValue.replace(/"/g, '\\"') + '"';
      }
      variableCheckValue = rawValue; // grader aspetta la stringa senza virgolette
    } else {
      // Number: proviamo a convertire a numero
      var n = Number(rawValue);
      if (isNaN(n)) {
        // se non è un numero valido, usiamo 0 come fallback e avvertiamo in console
        console.warn("Valore fornito non è un numero valido, uso 0 come fallback.");
        n = 0;
      }
      valueText = String(n);
      variableCheckValue = n;
    }

    var initial = template.replace('VALUE', valueText);

    // se esiste già un widget, potremmo volerlo rimpiazzare:
    // (alcune implementazioni di ParsonsWidget supportano re-init; per sicurezza creiamo un nuovo oggetto)
    parsonsPuzzle = new ParsonsWidget({
      "sortableId": "js_esgroup2_1-sortable",
      "max_wrong_lines": 10,
      "grader": ParsonsWidget._graders.VariableCheckGrader,
      "exec_limit": 2500,
      "can_indent": true,
      "x_indent": 50,
      "lang": "en",
      "show_feedback": true,
      "trashId": "js_esgroup2_1-sortableTrash",
      "variable_check": {
          "numero": variableCheckValue
      }
    });

    parsonsPuzzle.init(initial);
    parsonsPuzzle.shuffleLines();
  }

  // Inizializza con valore di default (5)
  createWidget("5", "number");

  // handler per il bottone set value
  document.getElementById("js_esgroup2_1-setValue").addEventListener("click", function(event){
    event.preventDefault();
    var raw = document.getElementById("js_esgroup2_1-valueInput").value;
    var type = document.getElementById("js_esgroup2_1-valueType").value;
    // se l'input è vuoto non cambiare (opzionale: qui ricreiamo comunque con fallback)
    if (raw === "") {
      if (type === "number") raw = "0";
      else raw = "";
    }
    createWidget(raw, type);
  });

  // reset/shuffle e feedback mantengono il comportamento precedente
  document.getElementById("js_esgroup2_1-newInstanceLink").addEventListener("click", function(event){
      event.preventDefault();
      if (parsonsPuzzle) parsonsPuzzle.shuffleLines();
  });
  document.getElementById("js_esgroup2_1-feedbackLink").addEventListener("click", function(event){
      event.preventDefault();
      if (parsonsPuzzle) parsonsPuzzle.getFeedback();
  });

})();
</script>

[Torna all'indice](../../../index.markdown)