---
layout: default
title: JavaScript - Esercizio gruppo 6 n. 7
description: Stampa sulla console il risultato del confronto tra due numeri per verificare se il primo numero è minore o uguale del secondo.
---

<div id="js_es1-6-sortableTrash" class="sortable-code"></div> 
<div id="js_es1-6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_es1-6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_es1-6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "function confrontaMinoreUguale(x, y) {\n" +
    "  if (x &lt;= y) {\n" +
    "    console.log(`${x} è minore o uguale a ${y}`);\n" +
    "  } else {\n" +
    "    console.log(`${x} è maggiore di ${y}`);\n" +
    "  }\n" +
    "}\n" +
    "// Esempi\n" +
    "confrontaMinoreUguale(3, 10);\n" +
    "confrontaMinoreUguale(12, 4);\n" +
    "function bool confrontaMinoreUguale(x, y) { #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_es1-6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_es1-6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_es1-6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_es1-6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>