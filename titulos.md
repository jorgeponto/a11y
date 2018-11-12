voltar ao [sumário](README.md)

# 2. Títulos e subtítulos

<table>
<caption>Lista de verificação para <strong>títulos e subtítulos</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>a) existe um título <code>&lt;h1&gt;</code> marcado na página?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) existe uma marcação hierarquizada de títulos e subtítulos na página (<code>&lt;h1&gt;...&lt;h6&gt;</code>)?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>
<h2 id="headings">Headings</h2>
<p>Web pages often have sections of information separated by visual headings, for example, heading text is bigger and bold (like &quot;Headings&quot; right above this sentence :-). To make these work for everyone, the headings need to be <a href="#markup" class="termref">marked up</a>. That way people can navigate to the headings — including people who cannot use a mouse and use only the keyboard, and people who use a screen reader.</p>
<p class="listintro">Heading levels should have a meaningful hierarchy, e.g.: </p>
<ul class="listafterpul listtight">
  <li>Heading Level 1 &lt;h1&gt;
    <ul>
      <li>Heading Level 2 &lt;h2&gt;
        <ul>
          <li>Heading Level 3 &lt;h3&gt;</li>
          <li>Heading Level 3 &lt;h3&gt;</li>
        </ul>
      </li>
      <li>Heading Level 2 &lt;h2&gt;
        <ul>
          <li>Heading Level 3 &lt;h3&gt;
            <ul>
              <li>Heading Level 4 &lt;h4&gt;</li>
              <li>Heading Level 4 &lt;h4&gt;</li>
            </ul>
          </li>
        </ul>
      </li>
      <li>Heading Level 2 &lt;h2&gt; </li>
    </ul>
  </li>
</ul>
<h3 class="whathead" id="headingswhattocheck">What to check for:</h3>
<ul>
  <li>The page has a heading. In almost all pages there should be at least one heading.</li>
  <li>All text that looks like a heading is marked up as a heading.</li>
  <li>All text that is marked up as a heading is really a conceptual section heading.</li>
  <li>The heading  hierarchy is meaningful. Ideally the page starts with an &quot;h1&quot; — which is usually similar to the page title — and does not skip levels; however, these are not absolute requirements.</li>
</ul>
<h3>Headings checks</h3>
<p class="listintro">The checks below provide instructions with different browsers for how to get an outline from headings or headings markup in a page.</p>
<p>Headings outline: an outline of the headings that are marked up on page, for example:</p>
<figure class="shrink-wrap">
  <div class="figcontent"><img src="/WAI/content-images/preliminary/headings-outline.png" alt="" width="674" height="263" /></div>
  <figcaption class="figcaption">Figure: Outline of headings.</figcaption>
</figure>
<p>Headings markup in page: a view of the page with the heading markup shown, for example:</p>
<figure class="shrink-wrap">
  <div class="figcontent"><img src="/WAI/content-images/preliminary/headings-in-page.png" alt="" width="674" height="230" /></div>
  <figcaption class="figcaption">Figure: Heading markup in page.</figcaption>
</figure>
<details><summary>
    <h4>To check headings <em>with WebDev toolbar</em></h4>
  </summary>
  <div>
    <h5 class="listintro">Headings outline:</h5>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Information&quot;, then &quot;View Document Outline&quot;.Or, with the keyboard: Alt+T, W (to Web Developer Extension), I, M<br />
      <em>A new page opens with the outline</em>. </li>
    <li>Non-visual checks:
      <ul>
        <li>Are headings listed. If there are no headings marked up, it will say &quot;0 headings&quot;.</li>
        <li>Does the outline start with [H1] and follow a meaningful hierarchy? (That&#39;s not required, but strongly suggested.)</li>
      </ul>
    </li>
    <li>Visual checks: Compare the Document Outline to the visual rendering of the page.
      <ul>
        <li>Are the things that look like headings on the page listed in the Document Outline?</li>
        <li>Are there things in the Document Outline that aren&#39;t really headings? </li>
      </ul>
    </li>
  </ol>
    <h5 class="listintro">Heading markup in the page: </h5>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Outline&quot;, then &quot;Show Element Tags Names When Outlining&quot;. Or, with the keyboard: Alt+T, W (to Web Developer Extension), O, S<br />
    </li>
    <li>In the toolbar, select &quot;Outline&quot;, then &quot;Outline Headings&quot;. Or, with the keyboard: Alt+T, W (to Web Developer Extension), O, H<br />
      <em>The headings will be outlined and &lt;h1&gt;, &lt;h2&gt;, etc. icons will be before the headings.</em> </li>
    <li>Anything that is a functional heading should have a heading icon before it.</li>
    <li>Anything that is a <b>not</b> functional heading should <b>not</b> have a heading icon before it.</li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>To check headings <em>with IE WAT</em></h4>
  </summary>
  <div>
    <h5 class="listintro">Headings outline:</h5>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Structure&quot;, then &quot;Heading Structure&quot;. Or, with the keyboard: Ctrl/cmd+Alt+6, then down arrow  to &quot;Heading structure&quot;.<br />
      <em>A new page opens with the outline.</em> </li>
    <li>Non-visual checks:
      <ul>
        <li>Are headings listed? If there are no headings marked up, it will say &quot;0 headings&quot;.</li>
        <li>Does the outline start with [H1] and follow a meaningful hierarchy? (That&#39;s not required, but strongly suggested.)</li>
      </ul>
    </li>
    <li>Visual checks: Compare the Document Outline to the visual rendering of the page.
      <ul>
        <li>Are the things that look like headings on the page listed in the Document Outline?</li>
        <li>Are there things in the Document Outline that aren&#39;t really headings? </li>
      </ul>
    </li>
  </ol>
    <h5 class="listintro">Heading markup in the page:</h5>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Structure&quot;, then &quot;Headings&quot;. Or, with the keyboard: Ctrl/cmd+Alt+6, then down arrow  to &quot;Headings&quot;.<br />
      <em>Headings will be surrounded with &lt;h1&gt;, &lt;h2&gt;, etc. icons in purple text on a light background.</em></li>
    <li>Anything that is a functional heading should have a heading icon before it.</li>
    <li>Anything that is a <b>not</b> functional heading should <b>not</b> have a heading icon before it.</li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>To check headings <em> in any browser</em></h4>
  </summary>
  <div>
    <h5 class="listintro">Headings outline:</h5>
    <ol>
    <li>In any browser, open the <a href="http://validator.w3.org/">W3C HTML Validator (The W3C Markup Validation Service)</a>.</li>
    <li>In the Address field, type the URI (e.g., www.w3.org).</li>
    <li>Click the More Options link.</li>
    <li>Select the Outline checkbox.</li>
    <li>Click the Check button.<br />
      <em>The results page appears (with title starting either [Valid] or [Invalid]).</em> </li>
    <li>In the results page, near the top, at the end of the &quot;Jump to:&quot; line, click the Outline text link.</li>
    <li>Non-visual checks:
      <ul>
        <li>Is there anything there? If there is no text between &quot;Below is an outline for this document, automatically generated from the heading tags (&lt;h1&gt; through &lt;h6&gt;.)&quot; and &quot;If this does not look like a real outline...&quot; it means there are no headings marked up on the page.</li>
        <li>Does the outline start with [H1] and follow a meaningful hierarchy? (That&#39;s not required, but strongly suggested.)</li>
      </ul>
    </li>
    <li>Visual checks: Compare the Document Outline to the visual rendering of the page.
      <ul>
        <li>Are the things that look like headings on the page listed in the Document Outline?</li>
        <li>Are there things in the Document Outline that aren&#39;t really headings? </li>
      </ul>
    </li>
  </ol>
    <h5 class="listintro">Heading markup in the page:</h5>
    <ol>
    <li>Open <a href="http://wave.webaim.org/">WAVE</a> web accessibility evaluation tool.</li>
    <li>Type the website address in the box after &quot;Enter the URL of the web site you want to evaluate:&quot;</li>
    <li>Click the &quot;WAVE this page!&quot; button.<br />
      <em>Your web page will show up in the browser with lots of little icons on it.</em> </li>
    <li>Anything that is a functional heading should have a heading icon (<img src="/WAI/content-images/preliminary/h1.png" alt="H1 WAVE Tool Icon" />, <img src="/WAI/content-images/preliminary/h2.png" alt="H2 WAVE Tool Icon" />, <img src="/WAI/content-images/preliminary/h3.png" alt="H3 WAVE Tool Icon" />, etc.) before it.</li>
    <li>Anything that is a <b>not</b> functional heading should <b>not</b> have a heading icon before it.</li>
  </ol>
  </div>
</details>
<details><summary>
    <h4 id="bad-headings">To practice checking headings in BAD:</h4>
  </summary>
  <div>
    <h5 class="listintro">Headings outline:</h5>
    <ul>
    <li>Follow  one of the instructions under &quot;Headings outline&quot; above and use the accessible News page: <code><a href="https://www.w3.org/WAI/demos/bad/after/news">www.w3.org/WAI/demos/bad/after/news</a></code>. Notice there is a nice hierarchical outline.</li>
    <li>Next, use the inaccessible News page: <code><a href="https://www.w3.org/WAI/demos/bad/before/news">www.w3.org/WAI/demos/bad/before/news</a></code>. (In HTML Validator, the &quot;Check&quot; button might now say &quot;Revalidate&quot;.) Notice there is just one heading.</li>
  </ul>
    <h5 class="listintro">Heading markup in the page:</h5>
    <ul>
    <li>Start by visually looking at the inaccessible BAD news page: <a href="https://www.w3.org/WAI/demos/bad/before/news.html"><code>www.w3.org/WAI/demos/bad/before/news</code></a>. What looks like headings? <i>(Citylights News, Heat wave linked to temperatures, Man Gets Nine Months in Violin Case, ...)</i></li>
    <li>Next, see how it should look. Follow one of the instructions for &quot;Heading markup in the page&quot; above on the accessible News page: <code><a href="https://www.w3.org/WAI/demos/bad/after/home">www.w3.org/WAI/demos/bad/after/home</a></code>. Notice the headings have icons next to them.</li>
    <li>Next, see what it looks like when headings are not marked up. Use the inaccessible News page: <code><a href="https://www.w3.org/WAI/demos/bad/before/home">www.w3.org/WAI/demos/bad/before/home</a></code>. Notice there is text that visually looks like headings, but does not have headings icons next to it. (With WAVE, there are yellow icons with &quot;h?&quot; because it thinks these might be headings.)</li>
  </ul>
  </div>
</details>
<details><summary>
    <h3 id="headingsmore">Learn more about headings</h3>
  </summary>
  <div>
    <ul>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">Info and Relationships</a> - Understanding Success Criterion 1.3.1 for WCAG 2.0 (Level A)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html">Headings and Labels</a> - Understanding Success Criterion 2.4.6 for WCAG 2.0 (Level AA)</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-headings.html">Section Headings</a> - Understanding Success Criterion 2.4.10 for WCAG 2.0 (Level AAA)</li>
  </ul>
  </div>
</details>
