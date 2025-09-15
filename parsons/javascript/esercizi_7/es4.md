---
layout: default
title: JavaScript - Esercizio gruppo 7 n. 4
---

<div id="js_esgroup7_4-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup7_4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup7_4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup7_4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let punteggio = prompt(&quot;Inserisci il punteggio dello studente:&quot;);\n" +
    "punteggio = Number(punteggio); // trasformo in numero\n" +
    "if (punteggio &gt;= 90) {\n" +
    "  console.log(&quot;Livello: A&quot;);\n" +
    "} else if (punteggio &gt;= 80) {\n" +
    "  console.log(&quot;Livello: B&quot;);\n" +
    "} else if (punteggio &gt;= 70) {\n" +
    "  console.log(&quot;Livello: C&quot;);\n" +
    "} else {\n" +
    "  console.log(&quot;Livello: D&quot;);\n" +
    "}\n" +
    "let messaggio = &quot;Controllo del punteggio...&quot;; #distractor\n" +
    "console.log(messaggio); #distractor\n" +
    "let bonus = 5; #distractor\n" +
    "let livelloProvvisorio = &quot;???&quot;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup7_4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup7_4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup7_4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup7_4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)