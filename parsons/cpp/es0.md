---
layout: default
title: C++ - Esercizio introduttivo n. 1
description: Crea un programma C++ che mostra un messaggio "Hello, world!" sulla console.
---

<div id="cpp_intro-1-sortableTrash" class="sortable-code"></div>
<div id="cpp_intro-1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="cpp_intro-1-feedbackLink" value="Get Feedback" type="button" />
    <input id="cpp_intro-1-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "#include &lt;iostream&gt;\n" +
    "using namespace std;\n" +
    "\n" +
    "int main() {\n" +
    "    cout &lt;&lt; &quot;Hello, world!&quot; &lt;&lt; endl;\n" +
    "    return 0;\n" +
    "}";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "cpp_intro-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#cpp_intro-1-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#cpp_intro-1-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

[Torna all'indice](../../../index.markdown)