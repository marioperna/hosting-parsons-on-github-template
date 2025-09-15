---
layout: default
title: JavaScript Dinamico - Esercizio 1.6
---

<div id="jsDinamico_es1-6-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "    &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;\n" +
    "    &lt;title&gt;Esercizio: Primo Elemento Figlio&lt;/title&gt;\n" +
    "    &lt;style&gt;\n" +
    "        #contenitore {...}\n" +
    "        .figlio {....}\n" +
    "    &lt;/style&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "    &lt;h1&gt;Esercizio: Ottenere il primo elemento figlio di un elemento padre&lt;/h1&gt;\n" +
    "    &lt;div id=&quot;contenitore&quot;&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Primo figlio&lt;/p&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Secondo figlio&lt;/p&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Terzo figlio&lt;/p&gt;\n" +
    "    &lt;/div&gt;\n" +
    "    &lt;button onclick=&quot;modificaPrimoFiglio()&quot;&gt;Modifica il primo figlio&lt;/button&gt;\n" +
    "    &lt;script&gt;\n" +
    "        function modificaPrimoFiglio() {\n" +
    "            const padre = document.getElementById(&#039;contenitore&#039;);\n" +
    "            const primoFiglio = padre.firstElementChild;\n" +
    "            primoFiglio.style.backgroundColor = &#039;lightblue&#039;;\n" +
    "            primoFiglio.style.fontWeight = &#039;bold&#039;;\n" +
    "            primoFiglio.textContent = &#039;Il primo figlio è stato modificato!&#039;;\n" +
    "        }\n" +
    "    &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "primoFiglio.text-content = &#039;Il primo figlio è stato modificato!&#039;; #distractor\n" +
    "const primoFiglio = padre.FirstElementChild; #distractor\n" +
    "const padre = getElementById(&#039;contenitore&#039;); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)