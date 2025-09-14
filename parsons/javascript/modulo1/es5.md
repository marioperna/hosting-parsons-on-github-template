---
layout: default
title: JavaScript Dinamico - Esercizio 1.5
---

<div id="jsDinamico_es1-5-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "    &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;\n" +
    "    &lt;title&gt;Esercizio: Ottenere Elementi Figli&lt;/title&gt;\n" +
    "    &lt;style&gt;\n" +
    "        #contenitore {\n" +
    "            border: 2px solid #333;\n" +
    "            padding: 10px;\n" +
    "            margin-bottom: 10px;\n" +
    "        }\n" +
    "        .figlio {\n" +
    "            margin: 5px 0;\n" +
    "            padding: 5px;\n" +
    "            border: 1px solid #999;\n" +
    "        }\n" +
    "    &lt;/style&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "    &lt;h1&gt;Esercizio: Ottenere tutti gli elementi figli di un elemento padre&lt;/h1&gt;\n" +
    "    &lt;div id=&quot;contenitore&quot;&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Figlio 1&lt;/p&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Figlio 2&lt;/p&gt;\n" +
    "        &lt;p class=&quot;figlio&quot;&gt;Figlio 3&lt;/p&gt;\n" +
    "    &lt;/div&gt;\n" +
    "    &lt;button onclick=&quot;evidenziaFigli()&quot;&gt;Evidenzia figli&lt;/button&gt;\n" +
    "    &lt;script&gt;\n" +
    "        function evidenziaFigli() {\n" +
    "            const padre = document.getElementById(&#039;contenitore&#039;);\n" +
    "            const figli = padre.children;\n" +
    "            for (let i = 0; i &lt; figli.length; i++) {\n" +
    "                figli[i].style.backgroundColor = &#039;yellow&#039;;\n" +
    "                figli[i].style.fontWeight = &#039;bold&#039;;\n" +
    "            }\n" +
    "        }\n" +
    "    &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "const figli = padre.childrens; #distractor\n" +
    "figli[i].backgroundColor = &#039;yellow&#039;; #distractor\n" +
    "figli[i].style.fontWeight: &#039;bold&#039;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-5-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>