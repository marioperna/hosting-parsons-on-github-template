---
layout: default
title: C++ - Esercizio condizionale n. 2
description: Creare if else in C++  
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
    "  int numero;\n" +
    "  cout &lt;&lt; &quot;Inserisci un numero: &quot;;\n" +
    "  cin &gt;&gt; numero;\n" +
    "  if (numero % 2 == 0){\n" +
    "    cout &lt;&lt; &quot;Il numero &egrave; pari&quot;;\n" +
    "  } else {\n" +
    "    cout &lt;&lt; &quot;Il numero &egrave; dispari&quot;;\n" +
    "  }\n" +
    "}\n" +
    "if numero % 2 == 0 { #distractor\n" +
    "} else if numero % 2 != 0 { #distractor\n" +
    "} else { #distractor\n" +
    "} #distractor";
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