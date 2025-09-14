---
layout: default
title: JavaScript Dinamico - Esercizio 1.2
---


<div id="jsDinamico_es1-2-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "    &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;\n" +
    "    &lt;title&gt;Esercizio: Modifica Stile per Classe&lt;/title&gt;\n" +
    "    &lt;style&gt;\n" +
    "        .evidenzia {\n" +
    "            color: black;\n" +
    "            font-size: 16px;\n" +
    "            padding: 10px;\n" +
    "            border: 1px solid #ccc;\n" +
    "            margin-bottom: 10px;\n" +
    "        }\n" +
    "    &lt;/style&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "    &lt;h1&gt;Esercizio: Ottenere elemento per classe e modificare lo stile&lt;/h1&gt;\n" +
    "    &lt;p class=&quot;evidenzia&quot;&gt;Questo è il primo paragrafo.&lt;/p&gt;\n" +
    "    &lt;p class=&quot;evidenzia&quot;&gt;Questo è il secondo paragrafo.&lt;/p&gt;\n" +
    "    &lt;p&gt;Questo paragrafo non cambierà.&lt;/p&gt;\n" +
    "    &lt;button onclick=&quot;modificaStile()&quot;&gt;Cambia stile dei paragrafi&lt;/button&gt;\n" +
    "    &lt;script&gt;\n" +
    "        function modificaStile() {\n" +
    "            // Otteniamo tutti gli elementi con la classe &#039;evidenzia&#039;\n" +
    "            const elementi = document.getElementsByClassName(&#039;evidenzia&#039;);\n" +
    "            \n" +
    "            // Modifichiamo lo stile di ciascun elemento\n" +
    "            for (let i = 0; i &lt; elementi.length; i++) {\n" +
    "                elementi[i].style.color = &#039;white&#039;;\n" +
    "                elementi[i].style.backgroundColor = &#039;blue&#039;;\n" +
    "                elementi[i].style.fontWeight = &#039;bold&#039;;\n" +
    "            }\n" +
    "        }\n" +
    "    &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "elementi[i].style.background-color = &#039;blue&#039;; #distractor\n" +
    "elementi[i].style.font-weight = &#039;bold&#039;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
