---
layout: default
title: JavaScript - Esercizio introduttivo n. 2
description: Seleziona la riga corretta per dichiarare una variabile in JavaScript.
---

<div id="js_intro-2-sortableTrash" class="sortable-code"></div> 
<div id="js_intro-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_intro-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_intro-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let myVar = 5\n" +
    "let let = 5; #distractor\n" +
    "let return = 5;  #distractor\n" +
    "let return = 5;  #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_intro-2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_intro-2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_intro-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_intro-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)