---
layout: default
title: JavaScript Dinamico - Esercizio 1.1
---


<div id="jsDinamico_es1-1-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "  &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "  &lt;title&gt;Ottenere elemento per ID&lt;/title&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "  &lt;h2&gt;Esempio di accesso a un elemento per ID&lt;/h2&gt;\n" +
    "  &lt;p id=&quot;mioParagrafo&quot;&gt;Ciao! Questo è il contenuto del paragrafo.&lt;/p&gt;\n" +
    "  &lt;script&gt;\n" +
    "    const paragrafo = document.getElementById(&quot;mioParagrafo&quot;);\n" +
    "    const content = paragrafo.innerHTML;\n" +
    "    alert(content);\n" +
    "  &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "const paragrafo = document.getElementsById(&quot;mioParagrafo&quot;); #distractor\n" +
    "const content = paragrafo.innerHTML(); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)