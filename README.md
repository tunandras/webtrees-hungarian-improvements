# webtrees—Hungarian improvements
Source: latest stable (1.7.2) release of <a href="https://launchpad.net/webtrees" target="_blank" title="Opens in new tab.">webtrees</a>.
<h2>Various files</h2>
These are modified PHP files—containing improvements mostly to display on-screen names in <i>Hungarian</i> and <i>East Asian order</i> (see <a href="https://en.wikipedia.org/wiki/Personal_name#Lexical_order" target="_blank" title="Opens in new tab.">Lexical order</a>) if chosen language is Chinese (Simplified), Hungarian, or Vietnamese, where the surname has to be in front of given names—as discussed in <a href="https://www.webtrees.net/index.php/en/forum/help-for-ver-1-6-2/30143-name-order" target="_blank" title="Opens in new tab.">Name order</a> in <b>webtrees</b> forum. In the future (when translated) Japanese, Korean, and Chinese (Traditional) could get this feature as well. Beyond that these files include some text adjustments too.
<h2>Hungarian translation file</h2>
There are a couple of changes (new translations and corrections of some translated terms) in “hu.po” Hungarian translation file—thanks to Gyönyör János (published by <a href="https://github.com/fisharebest/webtrees/commit/e1c58e6fe3d32e19454598497bbc67d6b749d957" target="_blank" title="Opens in new tab.">fisharebest</a> on October 7).
<h2>Usage</h2>
<ul>
  <li>For security reasons save your affected original “.php”, “hu.po” and/or “hu.mo” files.</li>
  <li>Save listed files above to your computer.</li>
  <li>Convert “hu.po” file to “hu.mo” with a converter (for example <a href="http://poedit.net/" target="_blank" title="Opens in new tab.">Poedit</a> or <a href="https://weblate.org/en/" target="_blank" title="Opens in new tab.">Weblate</a>) and upload it to webtrees_folder/language/ folder to your server.</li>
  <li>Then upload the PHP files overwriting the originals in the relevant folders to your server.</li>
  <li>If you are not satisfied with the result, you can return to the original behavior by replacing the new files with the saved (old) ones.</li>
</ul>
