---
layout: default
title: JavaScript - Esercizio gruppo 6 n. 6
description: Stampa sulla console il risultato del confronto tra un numero e una stringa per verificare se sono diversi sia in valore che in tipo.
---

<div id="js_esgroup6_6-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup6_6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup6_6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup6_6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "const a = 10;\n" +
    "const b = &quot;10&quot;;\n" +
    "const c = 10;\n" +
    "console.log(a !== b); // true -&gt; diversi per tipo\n" +
    "console.log(a !== c); // false -&gt; uguali in valore e tipo\n" +
    "console.log(a !== b); // true -&gt; uguali per tipo #distractor\n" +
    "console.log(a !== c); // false -&gt; uguali in valore ma non per tipo #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup6_6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup6_6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup6_6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup6_6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>