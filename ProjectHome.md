php Tools for Groupwise, aka. PTG, provides a basic web interface to some Groupwise management tasks that are normally not easily handled by the native admin tools provided with Groupwise.

PTG uses the Groupwise SOAP interface, and the Trusted Application API to a allow Groupwise administrators or helpdesk personnel access to among others:

  * proxy settings (view, add, delete, modify)
  * junkmail junk/block/trust entries (view, delete, add, move)
  * rules (view, delete)
  * client settings (view, modify)
  * modular, expandable, automated tasks for maintenance and reports (proxy settings, junk entries, etc.)
  * folders and mailbox items viewing, and attachment downloading
  * and more...

View or full management access to all of these features can be assigned to roles. Application users can then be assigned roles that define what they can and cannot see or do. Includes extensive logging of application user actions for auditing purposes.

Status

  * v0.7.3 - small bugfixes for running on Windows, see CHANGES.TXT
  * v0.7.2 - mainly fixes
  * v0.7.1 - Groupwise 8.0.1, PHP5.3, more reports, and CAS Single-Sign-On support
  * v0.5.1 - Several bug fixes, and installation on Windows running Wampserver
  * v0.5.0 - the first beta release is out, August 3, 2008

This is tested primarily against Groupwise v8.0.1HP. Due to the large number of SOAP-related bug-fixes in that version, we recommend that you upgrade to this version.

Please find it in the files section. You will need both the latest ptg.tar.gz file and gwkeygen.zip files to get started. Untar the ptg file somewhere in your web server path, and read the INSTALL.TXT file for more. See WINDOWS.TXT for Windows installation. You will need to run GWKEYGEN.EXE on a Windows system to generate a keys for your domain.
[edit](edit.md)
Requirements

  * a Linux OS with
> > - Apache 2.2
> > - PHP 5.1
> > - PHP SOAP extensions
  * or a Windows OS with WAMPServer v2.0c (see wampserver.com), or XAMPP
  * Firefox with Javascript 1.5 (may work with IE, not tested extensively)
  * A Trusted Application key, which can be generated with the GWKEYGEN.EXE Windows application. See the file section below to download it. This requires the Visual Basic 6 runtime. (Sorry, only a Windows version exists. This is a Novell limitation as the Trusted Key Generation API is only implemented on Windows)

PTG is developed and tested on SUSE10, CentOS 5, and Windows 7 with XAMPP, using PDT and Eclipse