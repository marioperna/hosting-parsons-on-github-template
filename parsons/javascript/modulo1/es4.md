---
layout: default
title: JavaScript Dinamico - Esercizio 1.4
---


<div id="jsDinamico_es1-4-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_es1-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_es1-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_es1-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&quot;it&quot;&gt;\n" +
    "&lt;head&gt;\n" +
    "    &lt;meta charset=&quot;UTF-8&quot;&gt;\n" +
    "    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;\n" +
    "    &lt;title&gt;Esercizio: Nascondere Elementi con Selettore CSS&lt;/title&gt;\n" +
    "    &lt;style&gt;\n" +
    "        .nascondi {\n" +
    "            font-size: 18px;\n" +
    "            color: darkred;\n" +
    "            margin-bottom: 10px;\n" +
    "        }\n" +
    "    &lt;/style&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "    &lt;h1&gt;Esercizio: Ottenere tutti gli elementi con un selettore CSS e nasconderli&lt;/h1&gt;\n" +
    "    &lt;p class=&quot;nascondi&quot;&gt;Primo paragrafo da nascondere.&lt;/p&gt;\n" +
    "    &lt;p class=&quot;nascondi&quot;&gt;Secondo paragrafo da nascondere.&lt;/p&gt;\n" +
    "    &lt;p&gt;Questo paragrafo rimarrà visibile.&lt;/p&gt;\n" +
    "    &lt;button onclick=&quot;nascondiElementi()&quot;&gt;Nascondi i paragrafi&lt;/button&gt;\n" +
    "    &lt;script&gt;\n" +
    "        function nascondiElementi() {\n" +
    "            const elementi = document.querySelectorAll(&#039;.nascondi&#039;);\n" +
    "            elementi.forEach(function(el) {\n" +
    "                el.style.display = &#039;none&#039;;\n" +
    "            });\n" +
    "        }\n" +
    "    &lt;/script&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;\n" +
    "const elementi = document.querySelectorAll(&#039;#nascondi&#039;); #distractor\n" +
    "const elementi = document.querySelectorAll(&#039;?nascondi&#039;); #distractor\n" +
    "const elementi = document.querySelectorAll(&#039;_nascondi&#039;); #distractor\n" +
    "const elementi = document.querySelectorAll(&#039;nascondi&#039;); #distractor\n" +
    "el.style = &#039;none&#039;; #distractor\n" +
    "el.style.displayNone = true; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_es1-4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_es1-4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_es1-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_es1-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>