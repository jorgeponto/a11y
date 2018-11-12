voltar ao [sumário](README.md)

# 5. Gráficos e imagens-hiperligadas

<table>
<caption>Lista de verificação para <strong>gráficos e imagens-hiperligação</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>a) as imagens ou os gráficos dispõem de um texto alternativo curto (i.e. atributo <code>alt</code>)?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) os gráficos dispõem de uma descrição longa (p.e. a tabela de dados que deu origem ao gráfico)?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>c) as imagens-hiperligação dispõem de um texto alternativo capaz de cumprir a função de texto da hiperligação?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>
<h2 id="images">Image text alternatives (&quot;alt text&quot;)</h2>
<p>Text alternatives (&quot;alt text&quot;) convey the purpose of an image, including pictures, illustrations, charts, etc. Text alternatives are used by people who do not see the image. (For example, people who are blind and use screen readers can hear the alt text read out; and people who have turned off images to speed download or save bandwidth can see the alt text.)</p>
<p>The text should be functional and provide an equivalent user experience, not necessarily describe the image. (For example,  appropriate text alternative for a search button <img src="/WAI/content-images/preliminary/search-button.png" alt="" width="36" height="24" /> would be &quot;search&quot;, not &quot;magnifying glass&quot;.)</p>
<p class="listintro">You don&#39;t usually see the alt text on a web page, it is in the web page <a href="#markup" class="termref">markup</a> (like this:<br />
  <code>&lt;img src=&quot;pointer_to_image.png&quot; alt=&quot;here's where the alternative text goes&quot;&gt;</code>).<br />
  Every image should include <code>alt</code> in the markup.</p>
<ul>
  <li>If an image conveys information useful for interacting with or understanding the web page content, then it needs alternative text.</li>
  <li>If an image is just decorative and people don&#39;t need to know about the image, then it should have null alt (<code>alt=&quot;&quot;</code>).</li>
</ul>
<p>Automated tests can tell you if <code>alt</code> is missing. To determine if the alternative text is appropriate, you need to see the image and judge it in context.</p>
<h3 class="whathead">What to check for:</h3>
<ul class="listwithpul">
  <li>Every image has <code>alt</code> with appropriate alternative text.</li>
</ul>
<h3>Tips</h3>
<p>Appropriate alternative text is not an exact science. Some people prefer most images to have more detailed  description; and others prefer much less description.</p>
<details><summary>
    <h4 class="f_panelHead listintro">Appropriate alt text:</h4>
  </summary>
  <div>
    <ul class="listspaced">
    <li>The text needs to convey the same meaning as the image. That is, if someone cannot see the image, they get the important information from the image in the alternative text.</li>
    <li>Alternative text depends on context. For example, for an image of a dog on a kennel club website, the alt text might include the breed of the dog; however, the same image on a dog park website may be there just to make the page more attractive, and the image might not need any alt text (and should have null alt). One way to help think about appropriate alt text is: if you were helping someone read and interact with the web page and they cannot see it, what would you say about the image?</li>
    <li>Images that are functional — for example,  images that initiate actions (like submit buttons) and linked images (like in navigation) — need alt text that is the functional equivalent.</li>
    <li>If there is text in the image — for example,  in a logo — that text needs to be included in the alt text.<br />
    </li>
    <li>If the image has complex information  — such as charts or graphs — the image should have a short alt text to identify the image, and then the detailed description of the information should be provided elsewhere (for example, in a data table).</li>
  </ul>
  </div>
</details>
<details><summary>
    <h4 class="f_panelHead listintro">What is not needed in the alt text:</h4>
  </summary>
  <div>
    <ul class="listspaced">
    <li>If the image is not important for understanding the content — for example, it is just decoration or &quot;eye candy&quot; — it should have null alt (<code>alt=&quot;&quot;</code>). One way to help determine if an image should have null alt is to ask yourself: <em>If the image was removed, would the user still get all the information from the page?</em></li>
    <li>The alternative text does not need to include the words &quot;button&quot;, &quot;link&quot;, or &quot;image of&quot;. (Screen readers automatically provide that information.)</li>
    <li>If the image is sufficiently described in the text — for example, a simple diagram illustrating what&#39;s written in the web page text — it can have brief alt text such as &quot;Diagram of work flow as describe above.&quot;</li>
  </ul>
  </div>
</details>
<details><summary>
    <h4 class="f_panelHead listintro"><code>alt</code> attribute in HTML (not &quot;alt tag&quot;)</h4>
  </summary>
  <div>
    <p>In HTML (which is web page code, called <a href="#markup" class="termref">markup</a>), alt is an attribute of the image element, and other elements. (So &quot;alt tag&quot; is technically incorrect; the correct terminology is &quot;alt attribute&quot;, or you can say &quot;alt text&quot;.) It looks like this in markup: <code>&lt;img alt=&quot;WAI logo&quot; src=&quot;/wai/logo.png&quot;&gt;</code></p>
  </div>
</details>
<h3>Alt text checks</h3>
<p>There are three options to check alt text listed below. The first one is the easiest, if you have the IE WAT toolbar. If you don&#39;t have any toolbars, there is a check at the end for any browser.</p>
<details><summary>
    <h4>To check alt text <em>with IE WAT</em></h4>
  </summary>
  <div>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Images&quot;, then &quot;Show Images&quot;. Or, with the keyboard: Ctrl/cmd+Alt+4, then arrow down to &quot;Show Images&quot;<br />
      <figure class="shrink-wrap">
        <div class="figcontent"><img src="/WAI/content-images/preliminary/alt-ie.png" alt="" width="674" height="223" /></div>
        <figcaption class="figcaption">Figure:  IE WAT toolbar with 'Images' drop down and 'Show Images' highlighted.</figcaption>
      </figure>
      <em>If there are any images missing alt, a dialog box appears with the number of images without alt attributes.<br />
      The alt text will be displayed before the images in quotes on a light background.</em></li>
    <li>To check for missing alt: Look for the text &quot;NoAlt!&quot; (visually, or with find-in-page). If you find it, that means the following image is missing alt.</li>
    <li>To check if alt text is appropriate:<br />
      For each image, see if the alt text adequately conveys the information in the image it is next to, per the Tips above. </li>
  </ol>
  </div>
</details>
<details><summary>
    <h4 id="altff">To check alt text <em>with WebDev toolbar</em></h4>
  </summary>
  <div>
    <ol>
    <li>Open the web page you are checking.</li>
    <li>In the toolbar, select &quot;Images&quot;, then &quot;Outline Images&quot;, then &quot;Outline Images Without Alt Attributes&quot;. Or, with the keyboard: Alt+T, W (to Web Developer Extension), I, O, A<br />
      <em>Red boxes appear around any images missing alt.</em><br />
      <figure class="shrink-wrap">
        <div class="figcontent"><img src="/WAI/content-images/preliminary/alt-ff-missing.png" width="676" height="278" alt="" /></div>
        <figcaption class="figcaption">Figure:  WebDev toolbar menu, and red boxes around images.</figcaption>
      </figure>
    </li>
    <li>Note images without any alt text.</li>
    <li>In the toolbar, select &quot;Images&quot;, then &quot;Display Alt Attributes&quot;. Or, with the keyboard: Alt+T, W (to Web Developer Extension), I, A <br />
      <em>The alt text will be displayed before the images as white letters on a red background.</em><br />
      <figure class="shrink-wrap">
        <div class="figcontent"><img src="/WAI/content-images/preliminary/ff-toolbar-display-alt.png" alt="" width="674" height="175" /></div>
        <figcaption class="figcaption">Figure:  WebDev toolbar menu, and alt text displayed.</figcaption>
      </figure>
    </li>
    <li>For each image, see if the alt text adequately conveys the information in the image it is next to, per the Tips above.</li>
  </ol>
  </div>
</details>
<details><summary>
    <h4>To check alt text <em>with any browser</em></h4>
  </summary>
  <div>
    <ol>
    <li>Open <a href="http://wave.webaim.org/">WAVE</a> web accessibility evaluation tool web page.</li>
    <li>Type the website address in the box after &quot;Enter the URL of the web site you want to evaluate:&quot;</li>
    <li>Click the &quot;WAVE this page!&quot; button.<br />
      <em>Your web page will show up in the browser with lots of little icons on it.</em></li>
    <li>To check for missing alt: Look for the red alt icon (<img src="/WAI/content-images/preliminary/alt_missing.png" alt="Red Alt Missing WAVE Tool Icon" />), or search for the alt text &quot;ERROR: Missing alt text&quot;. If you find it, that means the following image is missing alt.</li>
    <li>To check if alt text is appropriate: <br />
      Look for the green alt icon (<img src="/WAI/content-images/preliminary/alt.png" alt="Green Alt Exists WAVE Tool Icon" />). Next to it is text on a light blue background; the alt text is in between the asterisks (*). See if that text adequately conveys the information in the image it is next to, per the Tips above.
      <figure class="shrink-wrap">
        <div class="figcontent"><img src="/WAI/content-images/preliminary/alt-wave5.png" alt="" width="676" height="314" /></div>
        <figcaption class="figcaption">Figure: WAVE showing alt text.</figcaption>
      </figure>
    </li>
  </ol>
  </div>
</details>
<details><summary>
    <h4 id="bad-alt">To practice checking alt text in BAD</h4>
  </summary>
  <div>
    <p>With one of the checks above, use the inaccessible home page <code><a href="https://www.w3.org/WAI/demos/bad/before/home">www.w3.org/WAI/demos/bad/before/home</a></code> <br />
    Notice: </p>
    <ul class="listwithpul">
    <li>Missing alt:
      <ul class="listwithpul">
        <li>There are lots of images without alt text. (Many of these are just decorative and should have null alt text, per the Tips above.)</li>
        <li>The weather image of the cloud and sun is missing alt.</li>
      </ul>
    </li>
    <li>Inappropriate alt text:
      <ul class="listwithpul">
        <li>Near the top, left, see the long alt text starting with &quot;Red dot with...&quot;. That description is way too detailed and includes unimportant information. The appropriate alt text in the accessible page is: &quot;Citylights: your access to the city.&quot;</li>
        <li>Near the bottom in the middle, see the image of text: &quot;(1)269C-H-O-K-E&quot;. The alt is 123456789, which is not equivalent.</li>
      </ul>
    </li>
    <li>Appropriate alt text:
      <ul class="listwithpul">
        <li>Near the top, see the W3C image; the alt text is: &quot;W3C logo&quot;.</li>
      </ul>
    </li>
  </ul>
  </div>
</details>
<details><summary>
    <h3>Learn more about alt text</h3>
  </summary>
  <div>
    <ul class="listwithpul">
    <li><a href="/WAI/fundamentals/accessibility-principles/#alternatives">Text alternatives for non-text content</a> is an easy introduction with links to more details</li>
    <li><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">Non-text Content</a> - Understanding Success Criterion 1.1.1 for WCAG 2.0 (Level A)</li>
    <li><a href="https://www.w3.org/WAI/tutorials/images/decision-tree/">An alt text decision tree</a></li>
  </ul>
  </div>
</details>
