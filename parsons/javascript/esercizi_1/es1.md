---
layout: default
title: JavaScript - Esercizio gruppo 1 n. 1
description: Crea un pagina che mostra un messaggio “I’m JavaScript - Internal” mediante un alert contenuto in uno script interno.
---

<div id="js_esgroup1_1-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup1_1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup1_1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup1_1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "alert(&quot;I&#039;m JavaScript - Internal&quot;);\n" +
    "var &quot;I&#039;m a JavaScript - Internal&quot;; #distractor\n" +
    "let txt = &quot;I&#039;m a JavaScript - Internal&quot;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup1_1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup1_1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup1_1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup1_1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)