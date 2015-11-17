# Webtrees—Hungarian improvements
The improvements below are made in the latest stable (1.7.2) release of Webtrees.
<h2>Various “individual” files</h2>
These are modified PHP files—containing improvements mostly to display on-screen names in localized order if language is Hungarian and they include some text adjustments as well.
<h2>Top surnames module</h2>
Fixes two issues:
<ul>
  <li>It determines and in certain cases uses the highest number of surname occurrences to get at least one row in the list because if the value in “Minimum number of occurrences” Family trees preferences field is higher than the number of top surname’s occurrences, a short message “No data available in table” appears in top surnames list sent by webtrees_folder/packages/datatables-1.10.7/js/jquery.dataTables.min.js JavaScript file without the possibility of translating (and only if presentation style is table; all other styles results no message at all).</li>
  <li>The “Minimum number of occurrences” input field from Family trees Preferences page is copied into the module’s configure form otherwise the user (for instance a member, who has privileges to configure the module) doesn’t understand why the number of names differs from the expected (input of add and remove surnames may also be inserted into the form to make this module independent from module statistics—anyway I detected some anomaly with them: the result was not the same in statistics and top surnames modules—after filling these fields in Family trees Preferences form).</li>
</ul>
<h2>Hungarian translation file</h2>
There are a couple of changes (new translations and corrections of some translated terms) in “hu.po” Hungarian translation file—thanks to Gyönyör János (published by <a href="https://github.com/fisharebest/webtrees/commit/e1c58e6fe3d32e19454598497bbc67d6b749d957" target="_blank" title="Opens in new tab.">fisharebest</a> on October 7).

<h2>Installation / Usage</h2>
<ul>
  <li>First—for security reasons—save your affected original “.php”, “hu.po” and/or “hu.mo” files.</li>
  <li>Download listed files above to your computer.</li>
  <li>Convert downloaded “hu.po” file to “hu.mo” with a converter (for example <a href="http://poedit.net/" target="_blank" title="Opens in new tab.">Poedit</a> or <a href="https://weblate.org/en/" target="_blank" title="Opens in new tab.">Weblate</a>) and upload it to webtrees_folder/language/ folder on the server.</li>
  <li>Then upload the PHP files overwriting the originals in the relevant folders on the server.</li>
  <li>If you are not satisfied with the result, you can return to the original saved files by replacing the new ones.</li>
</ul>
