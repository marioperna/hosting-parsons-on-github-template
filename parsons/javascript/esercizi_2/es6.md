---
layout: default
title: JavaScript - Esercizio gruppo 2 n. 6
description: Crea un programma che dichiara una variabile name e la imposta con il valore John. Successivamente crea una variabile admin e assegna ad essa il valore della variabile name. Infine mostra il valore della variabile admin
---



<div id="js_esgroup2_6-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup2_6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup2_6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup2_6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let name = &quot;John&quot;;\n" +
    "let admin = name;\n" +
    "console.log(admin);\n" +
    "let last_name = &quot;Russo&quot;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup2_6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup2_6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup2_6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup2_6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


[Torna all'indice](../../../index.markdown)