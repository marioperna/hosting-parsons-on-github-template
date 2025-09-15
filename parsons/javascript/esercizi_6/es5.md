---
layout: default
title: JavaScript - Esercizio gruppo 6 n. 5
description: Stampa sulla console il risultato del confronto tra un numero e una stringa per verificare se sono diversi.
---

<div id="js_esgroup6_5-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup6_5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup6_5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup6_5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "const numero = 5;\n" +
    "const stringa = &quot;5&quot;;\n" +
    "console.log(numero !== stringa);\n" +
    "console.log(numero !!== stringa);  #distractor\n" +
    "console.log(numero !=== stringa); #distractor\n" +
    "console.log(numero =! stringa); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup6_5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup6_5-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup6_5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup6_5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)