voltar ao [sumário](README.md)
# 8. Estrutura da página

<table>
<caption>Lista de verificação para <strong>estrutura da página</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>quando se retira a CSS, todos os elementos (x)HTML alinham à esquerda?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>a) quando se retira a CSS, a informação aparece numa ordem lógica?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) quando se retira a CSS, é possível reconhecer a semântica dos diversos elementos?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>c) quando se retira a CSS, a informação relevante permanece visível?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>d) a maquetização da página não é feita através do elemento <code>&lt;table&gt;</code>?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>

<h2 id="structure">Basic structure check</h2>
<p><em>While the other checks on this page focus on specific success criteria in WCAG 2.0, this check is more broad. It helps you understand how some people &quot;see&quot; the web page differently. For this basic structure check, you look at the web page without images, styles, and layout.</em></p>
<p>Web pages are often designed with multiple columns, sections, colors, and other visual  aspects that help organize information for people who see the page in its default display. However, some people do not see the page this way. People who are blind listen to the page with a screen reader or read it from a Braille display. Some people  with low vision and others change the way the page is displayed so they can read it; for example, change from multiple columns to one column, change the text size, and more.</p>
<p>An important issue is how the web page works when it is &quot;linearized&quot; into one column and the presentation is changed, as shown in the images below.</p>
<details><summary>
    <p id="limgs"><strong>Images showing linearized and changed display </strong><em>(click to show images)</em></p>
  </summary>
  <div>
    <p>The images below illustrate how a web page is displayed in 3 columns by default and how it can be changed.</p>
    <p class="listintro">Figure A shows the default display of three columns, with the navigation at the left.</p>
    <figure class="shrink-wrap">
    <div class="figcontent"><img src="/WAI/content-images/preliminary/lin-start.png" alt="" width="363" height="150" /></div>
    <figcaption class="figcaption">Figure A.</figcaption>
  </figure>
    <p>Figure B shows the page linearized into one column, with the navigation at the top. Figure C shows the page  linearized, with the navigation at the bottom. The order of the sections (e.g., navigation at top or bottom or elsewhere) depends on how the web page is developed &mdash; the user usually cannot control the order.</p>
    <div class="multifigs">
    <figure class="shrink-wrap">
      <div class="figcontent"><img src="/WAI/content-images/preliminary/lin-lin.png" alt="" width="359" height="278" /></div>
      <figcaption class="figcaption">Figure B.</figcaption>
    </figure>
    <figure class="shrink-wrap">
      <div class="figcontent"><img src="/WAI/content-images/preliminary/lin-awk.png" alt="" width="359" height="278" /></div>
      <figcaption class="figcaption">Figure C.</figcaption>
    </figure>
  </div>
    <p>Figure D shows the page linearized and with styles turned off. When you follow the <a href="#bschecks">Basic structure checks steps below</a>, your page will look like something like this:</p>
    <figure class="shrink-wrap">
    <div class="figcontent"><img src="/WAI/content-images/preliminary/lin-plain.png" alt="" width="359" height="266" /></div>
    <figcaption class="figcaption">Figure D.</figcaption>
  </figure>
    <p>Figure E shows the page changed by a person with low vision to make it more readable, for example, the main text is big, the footer text is very small, and the headings are a different color.</p>
    <figure class="shrink-wrap">
    <div class="figcontent"><img src="/WAI/content-images/preliminary/lin-lv.png" alt="" width="359" height="429" /></div>
    <figcaption class="figcaption">Figure E.</figcaption>
  </figure>
    <hr />

  </div>
</details>
<p>While it is useful to have an experienced screen reader user check web pages, anyone can get an initial idea of  potential accessibility barriers for screen reader users and others who change the way the page is presented. The steps below show you how to disable images, disable styles for how the page is usually displayed, and linearize the page to check the page structure.</p>
<p id="dtnote">Notes:</p>
<ul>
  <li>Data tables will not make sense when linearized &mdash; that's OK because  screen readers have functionality to make data tables usable (when they are marked up correctly).</li>
  <li>BAD provides a clear example of how the basic structure check reveals accessibility barriers. (It's also a bit funny, and we suggest you check it out, by following the <a href="#plainBAD">BAD instructions</a> below.)</li>
</ul>
<h3>What to do:</h3>
<p class="listintro">Get a basic structure view of the page by following the instructions under <a href="#structure">Basic structure checks</a> below to: </p>
<ul>
  <li> Turn off images and show the text alternatives.</li>
  <li>Turn off style sheets (CSS), which specifies how the page is displayed with layout, colors, etc.</li>
  <li>Linearize the page or the tables (depending on the toolbar).</li>
</ul>
<h3>What to check for:</h3>
<ul>
  <li>Check that the information makes sense when read in the order it is shown; for example, headings are right above the information they apply to.<br />
    <em>(Data tables do not need to make sense linearized, per the <a href="#dtnote">note</a> above.)</em></li>
  <li>Check that the alternative text provides adequate information for the missing images (per the <a href="#images">Image text alternatives</a> section above).</li>
  <li>Check that blocks of information have clear headings (see also the <a href="#headings">Headings</a> section above). When navigation, main content, and other sections have  good headings, it's easier for people to find their way around the information.</li>
</ul>
<h3 id="bschecks">Basic structure checks</h3>
<details><summary>
    <h4>To check basic structure <em>with IE WAT</em></h4>
  </summary>
  <div>
    <ol>
    <li> Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Images&quot;, then &quot;Remove Images&quot;.<br />
      Or, with the keyboard: Ctrl+Alt+4, then arrow down to &quot;Remove Images&quot;.</li>
    <li> In the toolbar, select &quot;CSS&quot;, then &quot;Disable CSS&quot;.<br />
      Or, with the keyboard: Ctrl+Alt+3, then arrow down to &quot;Disable CSS&quot;.</li>
    <li>In the toolbar, select &quot;Tables&quot;, then &quot;Linearize&quot;.<br />
      Or, with the keyboard: Ctrl+Alt+7, then arrow down to  &quot;Linearize&quot;.</li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>To check  basic structure <em>with WebDev toolbar</em></h4>
  </summary>
  <div>
    <ol>
    <li> Open the web page you are checking.</li>
    <li> In the toolbar, select &quot;Images&quot;, then &quot;Disable Images&quot;, then &quot;Disable All Images&quot;.<br />
      Or, with the keyboard: Alt+T, W (to Web Developer Extension), I, D, D.</li>
    <li> In the toolbar, select &quot;CSS&quot;, then &quot;Disable Styles&quot;, then &quot;Disable All Styles&quot;.<br />
      Or, with the keyboard: Alt+T, W (to Web Developer Extension), S, D, D.</li>
    <li>In the toolbar, select &quot;Miscellaneous&quot;, then &quot;Linearize Page&quot;.<br />
      Or, with the keyboard: Alt+T, W (to Web Developer Extension), M, I.<br />
    </li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>To check  basic structure <em>with any browser</em></h4>
  </summary>
  <div>
    <p class="listintro">Most browsers provide the option to turn off images and disable CSS from the menus. For example:</p>
    <ul>
    <li>In Opera:
      <ul>
        <li>View &gt; Images &gt; Show Images<br />
          or, Alt+V, I, S</li>
        <li>View &gt; Style &gt; User Mode<br />
          or, Alt+V, S, U<br />
        </li>
      </ul>
    </li>
    <li>In Safari:
      <ul>
        <li>If the Develop menu is not shown in the menu bar, turn it on:
          <ul>
            <li>In Safari preferences, click Advanced.</li>
            <li>Select the &quot;Show Develop menu in menu bar&quot; checkbox.</li>
          </ul>
        </li>
        <li>Develop &gt; Disable Images<br />
          or, Ctrl+F2, D, down arrow to Disable Images</li>
        <li>Develop &gt; Disable Styles<br />
          or, Ctrl+F2, D, down arrow to Disable Styles</li>
      </ul>
    </li>
  </ul>
  </div>
</details>
<details><summary>
    <h4 id="plainBAD">To practice checking  basic structure with BAD</h4>
  </summary>
  <div>
    <ol>
    <li>First use the Accessible Home Page <code><a href="https://www.w3.org/WAI/demos/bad/after/home">www.w3.org/WAI/demos/bad/after/home</a></code> with one of the checks above to turn off images, disable CSS, and linearize.<br />
      Skim down and notice that under &quot;Welcome to CityLights&quot; there are 3 article headlines with summary text under each headline.</li>
    <li>Next use the Inaccessible Home Page <code><a href="https://www.w3.org/WAI/demos/bad/before/home">www.w3.org/WAI/demos/bad/before/home</a></code> with one of the checks above to turn off images, disable CSS, and linearize.
      <ul>
        <li>Skim down to find &quot;Welcome to CityLights&quot;. Notice that it's much harder to find. That's because it's not <a href="#markup" class="termref">marked up</a> as a <a href="#headings">heading, per above</a>.</li>
        <li>Notice that the 3 article headings are together and the article text is together. (For fun, read the article text together.)</li>
      </ul>
    </li>
    <li>To check a form, use the Inaccessible Survey Page <a href="https://www.w3.org/WAI/demos/bad/before/survey"><code>www.w3.org/WAI/demos/bad/before/survey</code></a> (This example is easier to see with IE WAT.) Look at how the radio buttons are laid out. Then linearize.<br />
      Notice that that radio button labels are not with the buttons. (This is because the page uses layout tables incorrectly.)</li>
  </ol>
  </div>
</details>
