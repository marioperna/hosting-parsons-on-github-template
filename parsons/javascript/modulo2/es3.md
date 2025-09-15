---
layout: default
title: JavaScript Dinamico - Esercizio 1.3
---

<div id="jsDinamico_es1-3-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "    &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;\n" +
    "    &lt;title&gt;Esercizio: Modifica Testo con Selettore CSS&lt;/title&gt;\n" +
    "    &lt;style&gt;\n" +
    "        .messaggio {...}\n" +
    "    &lt;/style&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "    &lt;h1&gt;Esercizio: Ottenere elemento tramite selettore CSS e modificare il testo&lt;/h1&gt;\n" +
    "    &lt;p class=&quot;messaggio&quot;&gt;Testo originale del paragrafo.&lt;/p&gt;\n" +
    "    &lt;button onclick=&quot;cambiaTesto()&quot;&gt;Cambia il testo del paragrafo&lt;/button&gt;\n" +
    "    &lt;script&gt;\n" +
    "        function cambiaTesto() {\n" +
    "            const paragrafo = document.querySelector(&#039;.messaggio&#039;);\n" +
    "            paragrafo.textContent = &#039;Il testo è stato modificato con JavaScript!&#039;;\n" +
    "        }\n" +
    "    &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "const paragrafo = document.querySelector(&#039;#messaggio&#039;); #distractor\n" +
    "const paragrafo = document.querySelector(&#039;messaggio&#039;); #distractor\n" +
    "const paragrafo = document.querySelector(&#039;?messaggio&#039;); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)