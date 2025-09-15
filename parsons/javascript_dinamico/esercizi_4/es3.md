---
layout: default
title: JavaScript Dinamico - Esercizio gruppo 4 n. 3
description: Creare un nuovo elemento img e impostare l'attributo src e alt
---

<div id="jsDinamico_esgroup4_3-sortableTrash" class="sortable-code"></div> 
<div id="jsDinamico_esgroup4_3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jsDinamico_esgroup4_3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jsDinamico_esgroup4_3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let immagine = document.createElement(&quot;img&quot;);\n" +
    "immagine.src = &quot;https://example.com/immagine.jpg&quot;;\n" +
    "immagine.alt = &quot;Descrizione dell&#039;immagine&quot;;\n" +
    "document.body.appendChild(immagine);\n" +
    "let altezza = 100 * 2; #distractor\n" +
    "for (let i = 0; i &lt; 3; i++) { #distractor\n" +
    "  let num = i + 10; #distractor\n" +
    "  console.log(&quot;Contatore &quot;, num); #distractor\n" +
    "} #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jsDinamico_esgroup4_3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "jsDinamico_esgroup4_3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jsDinamico_esgroup4_3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jsDinamico_esgroup4_3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>