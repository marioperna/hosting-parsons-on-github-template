---
layout: default
title: JavaScript - Esercizio gruppo 2 n. 6
description: Dichiarare una variabile chiamata "numero" e assegnarle il valore 5. Mostrare il valore della variabile.
---

// usa variableCheckGrader

<div id="js_esgroup2_1-sortableTrash" class="sortable-code"></div>
<div id="js_esgroup2_1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="js_esgroup2_1-feedbackLink" value="Get Feedback" type="button" />
    <input id="js_esgroup2_1-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "let numero = 5;\n" +
    "console.log(numero);\n" +
    "let nome = &quot;Mario&quot;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
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
        "numero": 5
    }
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup2_1-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#js_esgroup2_1-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script> 

[Torna all'indice](../../../index.markdown)