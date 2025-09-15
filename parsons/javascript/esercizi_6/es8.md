---
layout: default
title: JavaScript - Esercizio gruppo 6 n. 8
description: Stampa sulla console il risultato del confronto tra due numeri per verificare se il primo numero è diverso dal secondo.
---

<div id="js_esgroup6_8-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup6_8-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup6_8-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup6_8-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "const x = 10;\n" +
    "const y = 10;\n" +
    "if (x !== y) {\n" +
    "  console.log(`${x} è diverso da ${y}`);\n" +
    "} else {\n" +
    "  console.log(`${x} è uguale a ${y}`);\n" +
    "}\n" +
    "if (x !=== y) { #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup6_8-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup6_8-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup6_8-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup6_8-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>