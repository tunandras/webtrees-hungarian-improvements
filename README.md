# webtrees—Hungarian improvements
The source was the latest stable (1.7.2) release of <a href="https://launchpad.net/webtrees" target="_blank" title="Opens in new tab.">webtrees</a>.
<h2>Various files</h2>
These are modified PHP files—containing improvements mostly to display on-screen names in localized order if language is Hungarian (beyond that they include some text adjustments). According to the Hungarian rules the surname has to be in front of given names even in Edit name form or in autocomplete lists. Because of <i>Eastern order</i> rule (see chapter <a href="https://en.wikipedia.org/wiki/Personal_name#Lexical_order" target="_blank" title="Opens in new tab.">Lexical order</a> in article “Personal name” on Wikipedia) the same happens if language is Vietnamese or Chinese (Simplified)—as I saw in the forum of <b>webtrees</b> in the discussion <a href="https://www.webtrees.net/index.php/en/forum/help-for-ver-1-6-2/30143-name-order" target="_blank" title="Opens in new tab.">Name order</a> in March this year. In the future (when translated) Japanese, Korean, and Chinese (Traditional) could get this feature as well.
<h2>Hungarian translation file</h2>
There are a couple of changes (new translations and corrections of some translated terms) in “hu.po” Hungarian translation file—thanks to Gyönyör János (published by <a href="https://github.com/fisharebest/webtrees/commit/e1c58e6fe3d32e19454598497bbc67d6b749d957" target="_blank" title="Opens in new tab.">fisharebest</a> on October 7).
<h2>Top surnames module</h2>
Fixes two issues:
<ul>
  <li>It determines and in certain cases uses the highest number of surname occurrences to get at least one row in the list because if the value in “Minimum number of occurrences” Family trees preferences field is higher than the number of top surname’s occurrences, a short message “No data available in table” appears in top surnames list sent by webtrees_folder/packages/datatables-1.10.7/js/jquery.dataTables.min.js JavaScript file without the possibility of translating (and only if presentation style is table; all other styles results no message at all).</li>
  <li>The “Minimum number of occurrences” input field from Family trees Preferences page is copied into the module’s configure form otherwise the user (for instance a member, who has privileges to configure the module) doesn’t understand why the number of names is not the expected (input of add and remove surnames may also be inserted into the form to make this module independent from module statistics. Anyway, I detected some anomaly with them: the result was not the same in statistics and top surnames modules—after filling these fields in Family trees Preferences form).</li>
</ul>
<h2>Installation / Usage</h2>
<ul>
  <li>First—for security reasons—save your affected original “.php”, “hu.po” and/or “hu.mo” files.</li>
  <li>Save listed files above to your computer.</li>
  <li>Convert “hu.po” file to “hu.mo” with a converter (for example <a href="http://poedit.net/" target="_blank" title="Opens in new tab.">Poedit</a> or <a href="https://weblate.org/en/" target="_blank" title="Opens in new tab.">Weblate</a>) and upload it to webtrees_folder/language/ folder on the server.</li>
  <li>Then upload the PHP files overwriting the originals in the relevant folders on the server.</li>
  <li>If you are not satisfied with the result, you can return to the original saved files by replacing the new ones.</li>
</ul>
