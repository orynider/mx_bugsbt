# mx_bugsbt
<p><b><font size="5">MXP</font><font size="5"> Module -
            bugsBT <br>
        <font size="2">v. 2.0.2</font></font></b></p>
      <p><span style="font-weight: bold"><span style="font-size: 16px; line-height: normal">Module</span></span>
        <br />
        - for Mx Portal v. 2.7.5+ (with some notes, see below)</p>
      <p><strong>Author</strong><br />
        Haplo<br />
        <br />
        <span style="font-weight: bold">Description</span> <br />
        The MXP Module is an addon product for the MXP Portal.</p>
      <p><strong>Features</strong> <br />
        Easy to use and install/uninstall module.</p>
      <p> <br />
        I. <a href="#install">Installation instructions</a> <br />
        <br />
        II. <a href="#themes">Additional styles</a> <br />
        <br />
        III. <a href="#languages">Additional languages</a><br />
        <br />
        <a href="http://www.mx-publisher.com" target="_blank" class="postlink">DEMO
        </a> <br />
        <br />
        <a href="http://www.mx-publisher.com/index.php?page=4" target="_blank" class="postlink">
        DOWNLOAD </a> <br />
        <br /><a name="install">
        <br />
        <span style="font-weight: bold">I. Installation Instructions</span> <br />
        To install this module, follow these instructions. If you encounter any
        problems during install, visit the <a href="http://www.mx-publisher.com/forum/viewforum.php?f=20" target="_blank" class="postlink">
        module support forum</a>. </p>
      <p>All install notes are maintained at www.mx-publisher.com, <a href="http://www.mx-publisher.com/forum/viewforum.php?f=11">here</a>.<br>
        <br>
        <i>To summarize:</i></p>
      <ul>
        <li> If installing from scratch, use the &quot;install module&quot; option in the
            AdminCP - Modules</li>
        <li> If upgrading, use the &quot;upgrade module&quot; option in the
            AdminCP - Modules</li>
        <li> If uninstalling, use the &quot;delete module&quot; feature in the AdminCP
          - Modules</li>
      </ul>      <p><i>Note:</i> If upgrading, do NOT delete module prior to upgrading, or else
        you'll lose all module data!</p>
      <p><i>Note also:</i> Since this module is developed for next generation
        MXP core, you have to patch your core 2.7.5 portal if downloaded prior
        to this module release. If using latest core this patch is already included.</p>
      <p>OPEN admin/admin_mx_module.php</p>
      <p>FIND</p>
      <table width="100%" border="1" cellpadding="2">
        <tr>
          <td><font size="1">// <br>
// Generate safe object identifiers for the target DB<br>
// where this module pack is going to be imported...<br>
// </font></td>
        </tr>
      </table>      <p>BEFORE ADD</p>
      <table width="100%" border="1" cellpadding="2">
        <tr>
          <td><font size="1">// Start - For compatibility with MXP modules 2.x<br>
$fcontents_temp = array();<br>
for($i = 0; $i &lt; count($fcontents); $i++) {<br>
$module_data = explode($delimeter, trim($fcontents[$i]));<br>
<br>
if ( $module_data[0] != 'New_function' &amp;&amp; $module_data[4] != 'endoflist'
)<br>
{<br>
$fcontents_temp[] = implode($delimeter, $module_data);<br>
}<br>
}<br>
$fcontents = $fcontents_temp;<br>
// End - MXP modules 2.x code patch</font></td>
        </tr>
      </table>      <p><br />
        <a href="#top"> Back to Top</a> <br />
        <br />
        <a name="themes">
        <br />
        <span style="font-weight: bold">II. Additional Styles</span> <br />
        This module is compatible with any theme/style. <br />
        <br />
        <a href="#top"> Back to Top</a> <br />
        <br />
        <a name="languages">
        <br />
        <span style="font-weight: bold">III. Additional Languages</span> <br />
        First check to see if your language is already translated. <br />
        <br />
        Translated languages are downloaded <a href="http://www.mx-publisher.com/index.php?page=4&amp;action=category&amp;cat_id=5" target="_blank" class="postlink">
        here</a>. <br />
        <br />
        If exists, download and install in the modules/mx_modulename/language
                    folder. If not, duplicate (copy and paste) any included language
                  file, rename to match your language, translate using any texteditor,
                  save
                    and
                    upload. <br />
        <br />
                    <a href="#top"> Back to Top</a> </p>
      <p> /MXP Team</p>

