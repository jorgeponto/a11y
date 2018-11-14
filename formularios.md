voltar ao [sumário](README.md)

# 4. Formulários

<p>Muitas pessoas com deficiência visual ou deficiência motora interagem com a <em>web</em> (incluindo formulários) usando primeiramente um teclado em vez do rato. Como resultado, as suas interacções tendem a ser sequenciais pela ordem, amplamente controlada, como a página fora desenhada.</p>
<p>As etiquetas, o acesso por teclado, as instruções claras, e o manuseamento eficaz de erros são importantes para a acessibilidade de formulários.</p>
<p>Os campos de formulário e outros controlos de formulário têm normalmente etiquetas visiveis, por exemplo &quot;Endereço de E-mail:&quot; como etiqueta para um campo de texto</br>
<img src="http://www.w3.org/WAI/content-images/preliminary/form-label-text.png" width="242" height="29" alt="" class="imgbreathe" /><br />
<p>Quando estas etiquetas são marcadas corretamente, os utilizadores conseguem interagir utilizando apenas o teclado, o input de voz, e o leitor de ecrã. De igual forma, a própria etiqueta torna-se clicável, aumentando a área alvo e tornando mais fácil selecionar os pequenos <em>radio buttons</em> ou as <em>checkboxes</em>. Quando a marcação não é feita devidamente, uma pessoa cega, que utiliza o teclado, pode facilmente perder-se no formulário. </p>
  
<p> Um formulário pode ser uma única caixa de texto, tal como o campo de Pesquisa, ou pode ser um formulário complexo com campos de texto, radio buttons, checkboxes, listas drop-down, e botões.</p>  

<h4 class="small4">Labels</h4>
<ul>
  <li>Check that every form control has a label associated with it <span class="listintro"> using 'label', 'for', and 'id'</span>, as shown in the <a href="#labelschecks">labels checks</a> below. (This is best practice in most cases, though not a requirement because a form control label can be associated in other ways.)</li>
  <li>Check that the labels are positioned correctly. For left-to-right languages, labels should usually be:
    <ul>
      <li>Left of text boxes and drop-down lists.<br />
        <img src="/WAI/content-images/preliminary/form-label-text.png" width="242" height="29" alt="" class="imgbreathe" /></li>
      <li>Right of radio buttons and checkboxes. <br />
        <img src="/WAI/content-images/preliminary/form-label-radio.png" alt="" width="216" height="64" class="imgbreathe" /> </li>
    </ul>
  </li>
</ul>
<h4 class="small4">Required fields and other instructions</h4>
<ul>
  <li>Check that any fields that are required/mandatory are clearly indicated.
    <ul>
      <li>Check that the indicator does not rely on color alone, for example, if required fields were only indicated by red colored labels, they would not be accessible to people who do not see the different colors.</li>
      <li>Check that the indicator (such as asterisks (*)) is included in the marked up field label for text boxes and drop-down lists, or legend for  radio buttons and checkboxes, as shown in the <a href="#labelschecks">labels checks</a> below.</li>
    </ul>
  </li>
  <li>Check that any instructions for completing the form are before they are needed, for example,
    <ul>
      <li>General instructions should usually be at the top of the form or the section they relate to.</li>
      <li>Check that required formats, such as dates (year-month-date in the format 0000-00-00), are included in the marked up label, using the <a href="#labelschecks">labels checks</a> below.</li>
    </ul>
  </li>
</ul>
<h4 class="small4 listintro">Error handling</h4>
<p class="listintro spacenotop">Some simple forms, such as a single search field, might not have any errors. If you think the form(s) on the page you are checking might have error messages, try leaving required fields blank or entering incorrectly-formatted information (such as telephone number or e-mail address), then submitting the form. If you get errors:</p>
<ul>
  <li>Check that clear and specific guidance is provided to help people understand and fix the error. If the error concerns a format such as date, time, or address, check that the  correct format is clearly explained.</li>
  <li>Check that the errors are easily findable. Generally it is best if the error messages are before the form, rather than after the form.</li>
  <li>Check that the fields without errors are still populated with the data you entered. (This is best practice, though not a requirement.) People should not have to re-enter all the information in the form, except for some sensitive data such as credit card numbers.</li>
</ul>
<h3 id="labelschecks">Labels checks</h3>
<p><span class="listintro"><em><strong>Note:</strong></em> These instructions help you check  if labels are <a href="#markup" class="termref">marked up</a> with 'label', 'for', and 'id'; they do <strong>not</strong> check if  form controls are identified in other ways.</span> Therefore, even if a form does not pass these checks, it might still meet WCAG 2.0.</p>
<details><summary>
    <h4 id="labelsWAT">To check  labels <em>with IE WAT</em></h4>
  </summary>
  <div>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Structure&quot;, then &quot;FieldSet / Labels&quot;.
      Or, with the keyboard: Ctrl+Alt+6, then down arrow key to &quot;FieldSet / Labels&quot;, and select.
      <ul>
        <li> <em>A dialog box appears with the number of errors and controls.</em> <!-- <span class="changed">[@@ shall we explain &quot;to check out&quot;?] </span> --> 
          <br />
          <figure class="shrink-wrap">
            <div class="figcontent"> <img src="/WAI/content-images/preliminary/forms-wat-dialog.png" alt="" width="449" height="209" /> </div>
            <figcaption class="figcaption">Figure: IE WAT dialog box.</figcaption>
          </figure>
          <p><strong>The dialog box tells you the number of  identified errors, the total number of form controls, and the number of controls that you need to check manually. For the rest of the steps you need to look at the text around the labels. If this is difficult, you could skip the next steps.</strong></p>
        </li>
        <li><em>The form elements (labels and controls) are outlined in a red box, the markup is shown, and potential errors are indicated.<br />
          Example with no errors:</em><br />
          <figure class="shrink-wrap">
            <div class="figcontent"><img src="/WAI/content-images/preliminary/forms-wat-good.png" alt="" width="674" height="316" /></div>
            <figcaption class="figcaption">Figure: Form markup shown. Date label includes format.</figcaption>
          </figure>
          <em>Example with potential errors:</em><br />
          <figure class="shrink-wrap">
            <div class="figcontent"><img src="/WAI/content-images/preliminary/forms-wat-bad.png" alt="" width="674" height="305" /></div>
            <figcaption class="figcaption">Figure: Form markup shown. Date label does not include format. Fieldset missing legend.</figcaption>
          </figure>
        </li>
      </ul>
    </li>
    <li>Check that every field label has <code>label for=&quot;x&quot;</code> before it and <code>id=&quot;x&quot;</code> in the box with it, and that the text in quotes matches. <em>(&quot;x&quot; can be anything; for example, <code>for=&quot;park&quot;</code>, <code>id=&quot;park&quot;</code>)</em> 
      <!-- <span class="quiet">[@@ work with screen reader?]</span> -->
      <ul>
        <li>If the label is missing, it will indicate &quot;Label no for&quot;.</li>
        <li>If the <code>for</code> and <code>id</code> do not match, it will indicate &quot;input No Match id=&quot;x&quot;  Error&quot;.</li>
      </ul>
    </li>
    <li>Check that the required field indicator is in the field label, or for radio button and check boxes, it is in the &quot;legend&quot;. For example:
      <ul>
        <li>Correct: The asterisk (*) is included in the box around the label. 
          <!-- TODO Low Priority Add Image <span class="quiet">[image coming slh]</span> --> 
        </li>
        <li>Incorrect: The asterisk (*) is outside of the box around the label. 
          <!-- TODO Low Priority Add Image <span class="quiet">[image coming slh]</span> --> 
        </li>
        <li>Correct: &quot;(required)&quot; is in the legend. 
          <!-- TODO Low Priority Add Image <span class="quiet">[image coming slh]</span> --> 
        </li>
        <li>Incorrect: &quot;(required)&quot; is not in the legend. 
          <!-- TODO Low Priority Add Image <span class="quiet">[image coming slh]</span> --> 
        </li>
      </ul>
    </li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>Checking labels <em> with other browsers</em> </h4>
  </summary>
  <div>
    <p>There is not an easy way to check form control labels with the WebDev toolbar. There is a <a href="http://jimthatcher.com/favelets/">Form Labels favelet</a> that provides the same information as <a href="#labelsWAT">IE WAT above</a> and works with Firefox. It requires installation.</p>
  </div>
<h4 id="labelsmarkup">To check labels if you're comfortable looking at the <a href="#markup" class="termref">HTML markup</a></h4>
<div class="steps">
  <ol>
    <li>Open the source HTML and find the form markup.</li>
    <li>Check that:
      <ul>
        <li>Each form control has a <code>label</code> element with a <code>for</code> attribute that  matches the value of the <code>id</code> attribute in the related control. For example:<br />
          <code>&lt;label for=&quot;firstname&quot;&gt;First name: &lt;/label&gt;<br />
          &lt;input type=&quot;text&quot; name=&quot;firstname&quot; id=&quot;firstname&quot; /&gt;<br />
          </code> </li>
        <li>Each <code>id</code> is unique within the web page.</li>
      </ul>
    </li>
  </ol>
</div>
</details>
<details><summary>
    <h4 id="formsbad">To practice checking form labels and errors with  BAD</h4>
  </summary>
  <div>
    <h5 class="listintro">Labels:</h5>
    <ol>
    <li>Open the Accessible Survey Page: <a href="https://www.w3.org/WAI/demos/bad/after/survey">www.w3.org/WAI/demos/bad/after/survey</a> that has several forms. Do  the label  checks above.
      Notice the '<code>label</code>'s, '<code>for</code>'s, and '<code>id</code>'s.</li>
    <li>Open the Inaccessible Survey Page: <a href="https://www.w3.org/WAI/demos/bad/before/survey">www.w3.org/WAI/demos/bad/before/survey</a> and do the label checks above.<br />
      In IE WAT, you get the dialog box saying there are errors and the errors are marked in the page with  &quot;&lt;input    Error&gt;&quot;.</li>
  </ol>
    <h5 id="formerrorsbad">Errors:</h5>
    <ul>
    <li>Open the Accessible Survey Page: <a href="https://www.w3.org/WAI/demos/bad/after/survey">www.w3.org/WAI/demos/bad/after/survey</a>. Leave the fields blank and Submit the form.<br />
      Notice the error messages at the top and the asterisks to indicate required fields. Also, the page title includes &quot;Submission Failed&quot;.</li>
    <li>Open the Inaccessible Survey Page: <a href="https://www.w3.org/WAI/demos/bad/before/survey">www.w3.org/WAI/demos/bad/before/survey</a>. Leave the fields blank and Submit the form.<br />
      Notice errors are only indicated by the label being red, and there is no explanation of the errors.</li>
  </ul>
  </div>
</details>
<details><summary>
    <h3>Learn more about forms</h3>
  </summary>
  <div>
    <ul>
    <li> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-cues.html">Labels or Instructions</a> - Understanding Success Criterion 3.3.2 for WCAG 2.0 (Level A)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">Info and Relationships</a> - Understanding Success Criterion 1.3.1 for WCAG 2.0 (Level A)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-identified.html">Error Identification</a> - Understanding Success Criterion 3.3.1 for WCAG 2.0 (Level A)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-suggestions.html">Error Suggestion</a> - Understanding Success Criterion 3.3.3 for WCAG 2.0 (Level AA)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/minimize-error-reversible.html">Error Prevention (Legal, Financial, Data)</a> - Understanding Success Criterion 3.3.4 for WCAG 2.0 (Level AA) </li>
  </ul>
  </div>
</details>

<table>
<caption>Lista de verificação para <strong>formulários</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>a) ao clicar com o rato na etiqueta, o cursor aparece no campo de edição?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) é possível identificar os campos de preenchimento obrigatório quando usa apenas um leitor de ecrã?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>c) é possível ler facilmente as mensagens de erro usando apenas um leitor de ecrã?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>

