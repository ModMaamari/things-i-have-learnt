# Python -> Flask : 1- Inline if Statement in HTML:


```
{{ "value" if condition}}
```

Example:
In the next example I assumed that a dictionary xdic is passed from flask to the HTML template and I will use it to select a default value for a <select> tag

<pre><code>
<div class="form-group">
<label for="function">Function</label>
<select class="form-control" name ="function" id="function">
<option value = sin {{"selected" if xdic["sin"]}}>Sin</option>
<option value = cos {{"selected" if xdic["cos"]}}>Cos</option>
<option value = tan {{"selected" if xdic["tan"]}}>Tan</option>
<option value = cot {{"selected" if xdic["cot"]}}>Cot</option>
<option value = csc {{"selected" if xdic["csc"]}}>Csc</option>
</select>
</div>
</code></pre>

In the passed dictionary we should have only one function(sin or cos ... etc) that has True as its value.
