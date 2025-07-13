---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Multiple Parson's Problems on One Page
---
# Parsons Practice

## Parsons 1 (if-else)
Riordina i blocchi qui sotto in modo che stampino in modo corretto le indicazioni sulla temperatura.

<div id="p1exam-unibo-sortableTrash" class="sortable-code"></div> 
<div id="p1exam-unibo-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="p1exam-unibo-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="p1exam-unibo-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#include &lt;iostream&gt;\n" +
    "using namespace std;\n" +
    "int main(){\n" +
    "    int temperatura;\n" +
    "    string risultato = &quot;&quot;;\n" +
    "    cout &lt;&lt; &quot;Inserisci la temperatura \nesterna in gradi Celsius: &quot;;\n" +
    "    cin &gt;&gt; temperatura;\n" +
    "    if (temperatura &gt;= 30){\n" +
    "        risultato = &quot;Fa molto caldo oggi!&quot;;\n" +
    "    }\n" +
    "    else {\n" +
    "        risultato = &quot;La temperatura è piacevole oggi.&quot;;\n" +
    "    }\n" +
    "    cout &lt;&lt; risultato &lt;&lt; endl;\n" +
    "    return 0;\n" +
    "}\n" +
    "risultato = (temperatura &gt;= 30) : &quot;Fa molto caldo oggi!&quot; \n? &quot;La temperatura è sopportabile.&quot;; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "p1exam-unibo-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "p1exam-unibo-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#p1exam-unibo-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#p1exam-unibo-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

### Implementation Notes

When you host multiple Parson's problems on a single markdown page, you need to add a unique prefix. You can easily do this in the Codio generator by typing a unique prefix into the "Prefix" textbox and pressing Enter/Return. Then you can simply copy-paste like normal.

If want each problem to be it's own page, you can use relative path links at the bottom of each of your markdown pages as seen below. If you want students to be able to return to previous problems in this format, consider adding previous links or link to a table of contents like page.

### Example Next Link
[Next](./parsons/example1.html)
