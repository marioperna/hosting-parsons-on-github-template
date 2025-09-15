---
layout: default
title: JavaScript - Esercizio gruppo 10 n. 7
description: Scrivi una funzione che prenda una stringa come parametro e restituisca il numero di vocali presenti nella stringa.
---


<div id="js_esgroup10_7-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup10_7-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup10_7-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup10_7-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "function contaVocali(str) {\n" +
    "    let vocali = &quot;aeiouAEIOU&quot;;\n" +
    "    let count = 0;\n" +
    "    for (let i = 0; i &lt; str.length; i++) {\n" +
    "        if (vocali.includes(str[i])) {\n" +
    "            count++;\n" +
    "        }\n" +
    "    }\n" +
    "    return count;\n" +
    "}\n" +
    "// Esempio di utilizzo:\n" +
    "console.log(contaVocali(&quot;Ciao Mondo&quot;));\n" +
    "if (vocali.filters(str[i])) { #distractor\n" +
    "if (vocali.match(str[i])) { #distractor\n" +
    "if (vocali.strlen(str[i])) { #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup10_7-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup10_7-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup10_7-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup10_7-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)