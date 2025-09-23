---
layout: default
title: C++ - Esercizio condizionale n. 1
description: Creare if in C++
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
    "  int numero;\n" +
    "  cout &lt;&lt; &quot;Inserisci un numero: &quot;;\n" +
    "  cin &gt;&gt; numero;\n" +
    "  if (numero &gt; 0){\n" +
    "    cout &lt;&lt; &quot;Il numero &egrave; positivo&quot;;\n" +
    "  } else if (numero &lt; 0){\n" +
    "    cout &lt;&lt; &quot;Il numero &egrave; negativo&quot;;\n" +
    "  } else {\n" +
    "    cout &lt;&lt; &quot;Il numero &egrave; zero&quot;;\n" +
    "  }\n" +
    "}\n" +
    "if numero &gt; 0 { #distractor\n" +
    "} else if numero &lt; 0 { #distractor\n" +
    "} else if numero == 0 { #distractor\n" +
    "} else { #distractor\n" +
    "} #distractor";
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