---
layout: default
title: C++ - Esercizio introduttivo n. 1
description: Riordinare il seguente codice C++ in modo che stampi i numeri da 1 a 100.
---

<div id="cpp1-sortableTrash" class="sortable-code"></div> 
<div id="cpp1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="cpp1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="cpp1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int main(){\n" +
    "  int numero = 1;\n" +
    "  while (numero &lt;= 100){\n" +
    "    cout &lt;&lt; numero &lt;&lt; endl;\n" +
    "    numero++;\n" +
    "  }\n" +
    "}\n" +
    "int numero = 101; #distractor\n" +
    "numero &gt;= 100 #distractor\n" +
    "numero--; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "cpp1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "cpp1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#cpp1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#cpp1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


[Torna all'indice](../../../index.markdown)