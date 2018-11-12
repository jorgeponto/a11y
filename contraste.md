voltar ao [sumário](README.md)

# 6. Contraste

<table>
<caption>Lista de verificação de <strong>contrastes</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>a) para texto com tamanho normal, o rácio de contraste entre a cor do texto e a cor de fundo é superior a 4,5:1?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) para texto com tamanho grande, o rácio de contraste entre a cor do texto e a cor de fundo é superior a 3:1?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>

<h2 id="contrast"> Contrast ratio (&quot;color contrast&quot;)</h2>
<p>Some people cannot read text if there is not sufficient contrast between the text and background, for example,  light gray text on a light background.</p>
<figure class="shrink-wrap">
  <div class="figcontent"><img src="/WAI/content-images/preliminary/contrast-gray-white.png" alt="" width="301" height="127" /></div>
  <figcaption class="figcaption">Figure: Gray text on light background. </figcaption>
</figure>
<p>High contrast (for example, dark text on light background or bright text on dark background) is required by some people with visual impairments, including many older people who lose contrast sensitivity from ageing.</p>
<figure class="shrink-wrap">
  <div class="figcontent"> <img src="/WAI/content-images/preliminary/contrast-b-on-w.png" alt="" width="301" height="127" /> <img class="last-of-type" src="/WAI/content-images/preliminary/contrast-yellow.png" alt="" width="301" height="127" /> </div>
  <figcaption>Figure: Dark text on light background, and yellow text on black background.</figcaption>
</figure>
<!--figure-->
<p>While some people need high contrast, for others &mdash; including some people with  reading disabilities such as dyslexia &mdash;  bright colors (high luminance) are not readable. They need low luminance.</p>
<figure class="shrink-wrap">
  <div class="figcontent"><img src="/WAI/content-images/preliminary/contrast-lowlum1.png" alt="" width="301" height="127" /><img class="last-of-type" src="/WAI/content-images/preliminary/contrast-lowlum2.png" alt="" width="301" height="127" /></div>
  <figcaption>Figure: Brown text on dark background, and dark text on medium brown background.</figcaption>
</figure>
<!--figure-->
<p>Web browsers should allow people to change the color of text and background, and web pages need to work when people change colors.</p>
<p>(This accessibility requirement is sometimes called sufficient &quot;color contrast&quot;; however,  that is incorrect &mdash; technically it's &quot;luminance contrast&quot;. On this page we use &quot;contrast ratio&quot; as short for &quot;luminance contrast ratio&quot; because it's less jargony.) There is much more to know about contrast; we&#39;ve just introduced the basics here.</p>
<h3 class="whathead">What to check for:</h3>
<p>Web pages should also have a minimum contrast by default: a contrast ratio of at least 4.5:1 for normal-size text.</p>
<p class="listintro">There are basically three ways to check  contrast, each with strengths and weaknesses. </p>
<ol>
  <li><strong>Table with contrast ratio</strong> - The tool displays a table with all the possible contrast ratios in the web page. With some tools, you can click in the table and it will show where that color combination is in the web page.
    <ul>
      <li><em>Pro: </em>Comprehensive.</li>
      <li><em>Con: </em>Can be inaccurate, specifically, it can show some color combinations that are not really in the displayed page.</li>
    </ul>
  </li>
  <li><strong>Eye-dropper to select colors</strong> - The tool lets you select a text color and a background color, then it shows you the contrast ratio.<br />
    <ul>
      <li><em>Pro: </em>Accurate.</li>
      <li><em>Con: </em>Can only test one item at a time. Need to be able to see and use a mouse.</li>
    </ul>
  </li>
  <li><strong>Turn off color.</strong> The tool shows the page in grayscale.
    <ul>
      <li><em>Pro:</em> Gives you direct experience.</li>
      <li><em>Con: </em>Imprecise, does not provide contrast ratio value.</li>
    </ul>
  </li>
</ol>
<h3 id="contrastchecks">Contrast checks</h3>
<p>Below are instructions for checking contrast with IE WAT; a list of other contrast analyzer tools is in the <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html#visual-audio-contrast-contrast-resources-head">Related Resources section</a> of Understanding Success Criterion 1.4.3.</p>
<details><summary>
    <h4 id="contrastiewat">To check contrast <em> with IE WAT</em></h4>
  </summary>
  <div>
    <p>Here's how to do the three checks for sufficient contrast described above.</p>
    <ol>
    <li><strong>Table with contrast ratio</strong>:
      <ul>
        <li>In the toolbar, select  Color &gt; Juicy Studio Luminosity Analyser.
          Or, with the
          keyboard: Ctrl/cmd+Alt+5, then down arrow to &quot;Juicy Studio   Luminosity Analyser&quot;.<br />
          <img src="/WAI/content-images/preliminary/color-wat-table.png" alt="" width="700" height="72" class="imgbreathe" /><br />
          <em>A  new window  opens titled Colour Contrast Analyser with the table of results. The last column is Luminosity Contrast Ratio.</em></li>
      </ul>
    </li>
    <li><strong>Eye-dropper to select colors</strong>:
      <ul>
        <li>In the toolbar, select: Color &gt; Contrast Analyser [application]. Or, with the
          keyboard: Ctrl+Alt+5, then down arrow to &quot;Contrast Analyser [application]&quot;.<br />
          <em>The Color Contrast Analyser application window opens.</em><br />
        </li>
        <li>Using the first eye-dropper icon from the foreground color section, pick the foreground color (usually the text) you want to analyze.</li>
        <li> Using the second eye-dropper icon from the background color section, pick the corresponding background color.</li>
        <li><em>In the bottom of the Color Contrast Analyser window, the resulting luminosity Contrast ratio will show (for example: 7.5:1), along with &quot;Pass&quot; or &quot;Fail&quot; and a visual example of the colors.</em></li>
      </ul>
    </li>
    <li><strong>Turn off color:</strong>
      <ul>
        <li>In the toolbar, select  Color &gt; Grey Scale.  Or, with the
          keyboard: Ctrl+Alt+5, then down arrow to &quot;Gray Scale&quot;.</li>
        <li>Check if any information is lost or hard to see when  all colors are converted to grayscale.</li>
      </ul>
    </li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>Checking contrast <em>with other browsers</em></h4>
  </summary>
  <div>
    <p class="listintro">There is not an easy way to check contrast with the WebDev toolbar. There is a <a href="https://addons.mozilla.org/en-US/firefox/addon/juicy-studio-accessibility-too/">Juicy Studio Accessibility Toolbar</a> add-on that provides the same information as IE WAT above and works with Firefox.</p>
  </div>
</details>
<details><summary>
    <h4>To practice checking contrast with BAD</h4>
  </summary>
  <div>
    <p class="listintro">Open the  inaccessible Tickets page: <code><a href="https://www.w3.org/WAI/demos/bad/before/tickets.html">www.w3.org/WAI/demos/bad/before/tickets</a><br />
    </code>Use one of the checks above. Notice:</p>
    <ul>
    <li>The text in some rows is dark gray on light gray with a contrast ratio of 3.76:1.</li>
  </ul>
  </div>
</details>
<details><summary>
    <h3>Learn more about contrast ratio</h3>
  </summary>
  <div>
    <ul>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast">Contrast (Minimum)</a> - Understanding Success Criterion 1.4.3 for WCAG 2.0 (Level AA)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast">Contrast (Enhanced)</a> - Understanding Success Criterion 1.4.6 for WCAG 2.0 (Level AAA)<br />
    </li>
  </ul>
  </div>
</details>
