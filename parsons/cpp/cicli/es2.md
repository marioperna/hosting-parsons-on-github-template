---
layout: default
title: C++ - Esercizio introduttivo n. 2
description: Crea un programma C++ che sommi i numeri inseriti dall’utente fino a quando quest’ultimo non inserisce il valore 0.
---

<div id="cpp2-sortableTrash" class="sortable-code"></div> 
<div id="cpp2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="cpp2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="cpp2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int main(){\n" +
    "  int somma = 0;\n" +
    "  int numero;\n" +
    "  cout &lt;&lt; &quot;Inserisci un numero (0 per terminare): &quot;;\n" +
    "  cin &gt;&gt; numero;\n" +
    "  while (numero != 0){\n" +
    "    somma += numero;\n" +
    "    cout &lt;&lt; &quot;Inserisci un numero (0 per terminare): &quot;;\n" +
    "    cin &gt;&gt; numero;\n" +
    "  }\n" +
    "  cout &lt;&lt; &quot;La somma vale &quot; &lt;&lt; somma;\n" +
    "}\n" +
    "do (numero != 0) { #distractor\n" +
    "}while #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "cpp2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "cpp2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#cpp2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#cpp2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)