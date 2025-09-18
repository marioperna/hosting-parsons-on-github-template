---
layout: default
title: JavaScript - Esercizio gruppo 1 n. 2
description: Crea un pagina che mostra un messaggio “I’m JavaScript - Internal” mediante un alert contenuto in uno script esterno. N.B. Considera la presenza del file script.js contenga il codice JavaScript necessario per mostrare l’alert.
---

<div id="js_esgroup1_2-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup1_2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup1_2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup1_2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html&gt;\n" +
    "&lt;head&gt;\n" +
    "  &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "  &lt;title&gt;External JS&lt;/title&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "  &lt;script src=&quot;script.js&quot;&gt;&lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup1_2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup1_2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup1_2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup1_2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)