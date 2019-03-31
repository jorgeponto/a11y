<section id="checklist">

    <h2>Checklist</h2>
    
    <p>See also the <a href="assets/pdf/module-ios/module-ios-checklist.pdf" class="external" target="_blank">PDF version of the checklist. <img src="/assets/images/template/courses2014/new-window.png" alt="opens in a new window" class="new_window" width="13" height="13"></a></p>
    
<h3>User Interaction</h3>
<h4>Touch Target Size</h4>
<ul>
    <li>The click/touch target size SHOULD be large enough (without using zoom) to facilitate easy use with a finger, without risking activating an adjacent link or button.</li>
</ul>

<h4>Target Spacing and Grouping</h4>
<ul>
    <li>Touch targets MUST NOT overlap.</li>
    <li>      Compact touch targets SHOULD NOT be immediately adjacent to each other.    </li>
    <li>Active elements with the same target SHOULD be grouped into one touch target.</li>
</ul>

<h4>Activate on Release</h4>
<ul>
    <li>Touch controls MUST NOT activate when an item is first touched.</li>
</ul>

<h4>Kinetic/Accelerometer</h4>
<ul>
    <li>An application MUST NOT rely on kinetic motion (detected by the accelerometer) alone.</li>
    <li>The user SHOULD be able to disable motion-sensitive features.</li>
</ul>

<h4>Voice</h4>
<ul>
    <li>An application MUST NOT rely on voice control alone.</li>
</ul>

<h4>Gestures</h4>
<ul>
    <li>An application MUST NOT rely on gestures alone.</li>
    <li>Whenever possible, actions SHOULD be mapped to their corresponding default iOS gestures.</li>
  </ul>
<h3>UI Controls</h3>
<h4>Buttons</h4>
<ul>
  <li>A button MUST always convey its role using the correct trait.</li>
  <li>An active image used as a button MUST convey the correct role.</li>
  <li>When a button is disabled it MUST convey its state.</li>
</ul>
<h4>Links</h4>
<ul>
  <li>The role and purpose of a link MUST be clearly conveyed by VoiceOver.</li>
</ul>
<h4>Progress Bar</h4>
<ul>
  <li>Progress bars MUST convey their visible name to VoiceOver users with a descriptive, unique accessibility label.</li>
  <li>Progress spinners (UIActivityIndicatorView) MUST speak correct alternative text or immediately receive focus in order to convey an accessible name to VoiceOver users.</li>
</ul>
<h4>Slider</h4>
<ul>
  <li>Slider controls MUST have a visible label that is programmatically associated using the accessibility label property.</li>
</ul>
<h4>Switch</h4>
<ul>
  <li>Switch controls MUST have a visible label that is programmatically associated using the accessibility label property.</li>
  </ul>
<h3>Notifications</h3>
<h4>Notifying Users of Changes</h4>
<ul>
  <li>Dynamically generated content following user interaction MUST meet one of the following: assistive technology is automatically made aware of the new content OR the new content is the very next thing the assistive technology will encounter on the page.</li>
</ul>
<h4>Time Limits</h4>
<ul>
  <li>If there is a session time limit, users MUST be warned before the session ends and MUST be given time to save their data and/or extend the session.</li>
  <li>Incomplete data SHOULD be saved after a session timeout.</li>
</ul>
<h4>Alert</h4>
<ul>
  <li>Alerts MUST include a title and description.</li>
</ul>
<h4>Dialog</h4>
<ul>
  <li>Custom Dialogs MUST set <code>accessibilityViewIsModal</code> to "true" and the focus MUST be sent to the dialog.</li>
</ul>
<h3>Custom Elements</h3>
<h4>Accordion</h4>
<ul>
  <li>Accordion components MUST announce their accessible name and their expanded or collapsed state.</li>
</ul>
<h4>Autocomplete</h4>
<ul>
  <li>VoiceOver users MUST be automatically made aware of the autocomplete suggestions when they appear.</li>
</ul>
<h4>Rating</h4>
<ul>
  <li>A rating control MUST always convey its current value, any visible information, and be operable by both VoiceOver and non-VoiceOver users.</li>
</ul>
<h4>Sortable Table</h4>
<ul>
  <li>If a table is sortable, the header cells' accessibility labels MUST dynamically update to correctly convey their sorted state each time the data order changes.</li>
</ul>
<h4>Toggle</h4>
<ul>
  <li>Toggle buttons MUST convey an accessible name with programmatically associated, visible labels and convey their state using the accessibility label.</li>
  <li>Image toggle buttons MUST have descriptive, accurate alternative text provided in the accessibility label.</li>
</ul>
<h3>Form Labels and Validation</h3>
<h4>Labels</h4>
<ul>
  <li>The label MUST be visible at all times.</li>
  <li>Labels MUST be programmatically associated with their corresponding control elements.</li>
  <li>A "hint" SHOULD be provided when the label doesn't sufficiently convey a control's purpose to VoiceOver users.</li>
</ul>
<h4>Group Labels</h4>
<ul>
  <li>For groups of related controls where the individual labels for each control do not provide a sufficient description, additional group labels MUST be provided.</li>
</ul>
<h4>Checkboxes</h4>
<ul>
  <li>Checkboxes MUST convey their selected or checked state to VoiceOver.</li>
  <li>Groups of checkboxes MUST provide a common group label as well as a unique label for each control via their accessibility label properties.</li>
</ul>
<h4>Date Picker</h4>
<ul>
  <li>A standard Date Picker control SHOULD be used instead of a text field in order to avoid forcing users to enter a date with a default keyboard.</li>
</ul>
<h4>Radio Buttons</h4>
<ul>
  <li>Radio buttons MUST provide a common group label as well as a unique label for each control via their accessibility labels and they MUST convey their selected state.</li>
</ul>
<h4>Select (UIPickerView)</h4>
<ul>
  <li>Controls using UIPickerView MUST be programmatically associated with their visible label in order to provide an accessible name.</li>
</ul>
<h4>Text Fields</h4>
<ul>
  <li>Text fields MUST have programmatically associated, visible labels.</li>
</ul>
<h4>Validation and Error Reporting</h4>
<ul>
  <li>Efficient, intuitive, and clearly identified text based alerts MUST be provided to users for form validation cues and errors.</li>
  <li>If input errors are automatically detected, suggestions MUST be provided in text for fixing the input in a timely and accessible manner before the data is submitted to the server.</li>
</ul>

<h3>Navigation</h3>
<h4>Page Titles</h4>
<ul>
    <li>Screens MUST have meaningful titles.</li>
</ul>

<h4>Tab Panel</h4>
<ul>
    <li>Tabs MUST convey their role, their current state, and their order in the total number of tabs to VoiceOver users.</li>
</ul>

<h4>Menu</h4>
<ul>
    <li>Menu items MUST have the appropriate trait in order to convey their accessible role.</li>
    <li>The button that opens the menu MUST have a clear, descriptive title or accessibility label to accurately convey its purpose.</li>
    <li>VoiceOver users MUST be able to dismiss the menu.</li>
    <li>When the menu is closed, focus MUST return to the triggering button.</li>
  </ul>
<h3>Device Orientation</h3>
<ul>
  <li>The orientation of the content MUST not be locked to either landscape or portrait unless a specific orientation is essential for the functionality of the app.</li>
</ul>
<h3>Semantic Structure and Meaning</h3>
<h4>Headings</h4>
<ul>
    <li>Headings used to title or describe sections of content MUST use the header trait in order to convey their semantic purpose.</li>
</ul>

<h4>Tables</h4>
<ul>
    <li>Data tables MUST have the correct reading order, MUST convey the row and column header text for each data cell, and MUST correctly associate the data cell with the header cell in the accessibility label.</li>
</ul>

<h4>Reading Order and Focus Order</h4>
<ul>
    <li>The reading order of a screen as conveyed by VoiceOver MUST be logical and intuitive.</li>
    <li>When content is added or deleted from a screen, VoiceOver focus MUST be managed logically and never be lost.</li>
  </ul>
<h3>Color and Contrast</h3>
<h4>Colors that Convey Information</h4>
<ul>
  <li>Any information conveyed by color MUST be accompanied by a programmatically-discernible text alternative.</li>
  <li>The text alternative for information conveyed by color MUST accurately convey the same information without color.</li>
  <li>Any information conveyed by color MUST be accompanied by a visible alternative (text, image, etc.) that does not depend on color for meaning.</li>
  <li>Color alone MUST NOT be used to distinguish links from surrounding text unless the color contrast between the link and the surrounding text is at least 3:1. An additional differentiation (e.g. underline, outline, etc.) SHOULD BE provided as well.</li>
</ul>
<h4>Contrast</h4>
<ul>
  <li>Small text (under 18 point regular font or 14 point bold font) MUST have a contrast ratio of at least 4.5 to 1 with the background.</li>
  <li>Large text and images of large text (at or over 18 point or 14 point bold) MUST have a contrast ratio of at least 3 to 1 with the background.</li>
  <li>The contrast of UI control boundaries compared to adjacent areas SHOULD be sufficient (3 to 1 for UI control boundaries measuring at least 3px by 3px, and 4.5 to 1 for all other UI controls) to distinguish the UI control from the adjacent areas.</li>
  <li>Small text (under 18 point regular font or 14 point bold font) SHOULD have a contrast ratio of at least 7 to 1 with the background.</li>
</ul>
<h3>Animations and Motion</h3>
<h4>Parallax and Accelerometer Animations</h4>
<ul>
  <li>Moving the physical device SHOULD NOT cause non-essential visual motion or animations (e.g. parallax effects)</li>
  <li>Users MUST be able to disable any non-essential motion-sensitive visual effects.</li>
</ul>
<h4>Moving or Disappearing Content</h4>
<ul>
  <li>Automatically moving, blinking, or scrolling content that lasts longer than 5 seconds MUST be able to be paused, stopped, or hidden by the user.</li>
</ul>
<h4>Blinking or Flashing Content</h4>
<ul>
  <li>A screen MUST NOT contain content that flashes more than 3 times per second unless that flashing content is sufficiently small, and the flashes are of low contrast and do not violate general flash thresholds.</li>
</ul>
<h3>Audio and Video</h3>
<h4>Captions</h4>
<ul>
  <li>All prerecorded video MUST have synchronized captions.</li>
  <li>All live multimedia (video plus audio) events that contain dialog and/or narration MUST be accompanied by synchronized captions.</li>
  <li>Live audio consisting mainly of dialog and/or narration SHOULD have synchronized captions.</li>
</ul>
<h4>Transcripts</h4>
<ul>
  <li>All prerecorded video and audio MUST have text transcripts.</li>
</ul>

<h3>Text Content</h3>
<h4>Language Settings</h4>
<ul>
    <li>The language of the page MUST be programmatically identified.</li>
    <li>The language of sections of content that are different from the app's default language MUST be identified in such a way that they can be discovered by assistive technology.</li>
</ul>

<h4>Text Resize</h4>
<ul>
    <li>The screen MUST be readable and functional when text is set to 200% of its initial size.</li>
</ul>

<h4>Emojis</h4>
<ul>
    <li>Emojis MAY be used in text content.</li>
	<li>Custom emojis in custom keyboards MUST have alternative text.</li>
</ul>

<h3>Images</h3>
<h4>Alternative Text</h4>
<ul>
    <li>Images that convey information MUST have a descriptive accessibility label that serves the same purpose and presents the same information as the image.</li>
    <li>Images that are active MUST have an accessibility label that describes the purpose or function of the image.</li>
    <li>Images that are too complex to be fully described in a short text alternative MUST have their purpose described using an extended text alternative.</li>
    <li>Images that do not convey content, are decorative, or with content that is already conveyed in the text MUST NOT be given an alternative text equivalent that is exposed to assistive technology.</li>
</ul>

<h4>Text in Images</h4>
<ul>
    <li>An image MUST NOT include informative text if an equivalent visual presentation of the text can be rendered using real text.</li>
</ul>

</section>
