# Change Log
All notable changes to this project will be documented in this file.

## 2015-03
Contributors: [Luka Krajger](https://github.com/KLuka), [Philip Hughes](https://github.com/Grimthorr), [Daniel Gröber](https://github.com/DanielG), [Ezra Buehler](https://github.com/easybe), [Anders Kaseorg](https://github.com/andersk), [Jonathan Rennison](https://github.com/JGRennison), [Guillaume Martres](https://github.com/smarter)

	- Swap to gzip compression (fixes #262 and #266).

	- Set the encoding of .html files to UTF-8.

	- Fix <input> element type.

	- Issue #173: Keyboard icon on dark background.

	- Another (final) fix for Firefox keycodes problems.

	- Removed at sign (@) from beginning of some JS comments.

	- Issues #51, #202 ... : Keycodes fixes for FireFox.

	- Issue #195: A couple of bugs in vt100.jspp.

	- Issue #103, #203: Child process termination (partial fix).

	- Merge pull request #285 from KLuka/master.

	- Issue #275: gracefully manage HTTP time-outs and connection problems.

	- Set SSL options for increased security and disable compromised SSL
	version 2.0 and 3.0.

	- Issue #262: Page cannot be displayed.

	- Issue #180: Ever growing console occurs in iPad.

	- Issue #202: "-_" keys don't not work in FF > 15.

	- No longer set HTTP Content-Length.

	- Issue #245: Blank screen in Chrome 31.0.1650.57.

	- Issue #114: popup warning on tab/window close.

	- Issues 39, 43, 166 and 172 commits applied to .jspp files.

	- Removed auto-generated .js files.

## 2012-04  Marc Singer  <elf@woollysoft.com>

	- Fixing errors reported by piuparts.

	- Debian build now defaults to direct link with shared libraries.

	- Removing PATH_MAX reference.

	- Fixing Valgrind discovered issues.

	- Issue 172: autocorrect/autocapitalize can cause problems on
	mobile devices.

	- Issue 167: Accept connections in subfolders.

	- Issue 39: Clipboard not integrated with client operating system

	- Cleanup of debian control file before 2.11.

	- Issue 166: Color goes away.

	- Issue 167: Accept connections in subfolders.

## 2012-03  Marc Singer  <elf@woollysoft.com>

	- Issue 134: How to add arguments.

	- Issue 116: A shellinthebox runner / configuration file.

	- Issue 93: openssl required install-time.

	- Issue 50: SSH service not working on Centos/RHEL.

	- Issue 49: Debian packageing uses cross-directory hardlinks.

	- Issue 47: Does not build on Mac OSX.

	- Issue 43: 2.10 version introduces a keyboard layout problem.

	- Issue 39: clipboard not integrated with client operating system.

## 2012-02-02  Jay Weisskopf  <jay@jayschwa.net>

	- Use 2048-bit RSA keys for auto-generated certificates.

	- Assume a private key is RSA if the header does not specify a type.

## 2012-01-12  Anders Kaseorg  <andersk@mit.edu>

	- sslGenerateCertificate: Don't use the shell.

	- sslSNICallback: Properly disallow invalid characters.

	- Fix miscellaneous strncat buffer overflows.

## 2012-01-04  Jay Weisskopf  <jay@jayschwa.net>

	- Fixed an error in the init script's status function.

	- Check for null pointers from gethostbyname_r() to prevent seg faults.

## 2012-01-01  Jay Weisskopf  <jay@jayschwa.net>

	- Removed "Lucida Console" font because bold is wider than normal.

	- Bold and underline SGR attributes now utilize CSS.

	- Removed color pair restrictions.

	- Removed config.h. It is auto-generated by the configure script.

	- Changed the cursor color to match the default text color.

	- Write the OSC title to the window's title instead of the status bar. …

## 2010-10  Markus Gutschke  <markus@shellinabox.com>
	
	- Fixed inefficient I/O behavior and ability to interrupt long running
	output with CTRL-C.

	- Fixed confusing error message when we fail to dynamically load
	PAM support.

	- Fall back to calling select() instead of poll() for MacOS X.

## 2010-09  Markus Gutschke  <markus@shellinabox.com>

	- Implement a few work-arounds to avoid some problems with
	pututxline() on MacOS X.
 
	- Relax a check() that would trigger when using old-style
	(pre-Unix 98) pseudo terminals.

	- Another iteration of changes intended to deal with MacOS X
	specific build.

	- In an attempt to reduce build dependencies, remove the requirement
	for objcopy. Instead, we are now using "od" to generate C source code.

	- Added support for building with toolchains that don't support
	symbol aliasing.

	- Adjusted MIME types.

	- Store keyboard layout in separate HTML file.

## 2010-09-11  Markus Gutschke  <markus@shellinabox.com>

	- Added --pidfile= option that can be used even if running in the
	foreground.

## 2010-09-04  Markus Gutschke  <markus@shellinabox.com>

	- Added an optional on-screen keyboard. Must be activated by the
	user by selecting the option in the context-menu.

## 2010-09-03  Markus Gutschke  <markus@shellinabox.com>

	- Fix some scaling related issues. This fix is thanks to some
	excellent detective work by Jan <siev...@zedat.fu-berlin.de>.

	- Allow changing of font sizes in the user CSS.

## 2010-08-19  Markus Gutschke  <markus@shellinabox.com>

	- Thanks to lotr44's excellent analysis of the problem, we now have
	a fix for the problem with typing "!" on French keyboards.

## 2010-08-06  Markus Gutschke  <markus@shellinabox.com>

	- Allow users to disable the blinking cursor from the context menu.

## 2010-07-08  Markus Gutschke  <markus@shellinabox.com>

	- Added support for systems that have utmpx.h, but don't implement
	updwtmpx().

## 2010-07-02  Markus Gutschke  <markus@shellinabox.com>

	- Fixed a NULL pointer dereference that can occur when hostnames
	do not resolve. Thanks to <vmagerya> for pointing out this problem.

## 2010-03-31  Markus Gutschke  <markus@shellinabox.com>

	- Tweaked the build system to work better on OpenWRT. This is largely
	thanks to very helpful bug reports, and lots of testing by Jan Jaeger.

## 2010-03-29  Markus Gutschke  <markus@shellinabox.com>

	- Started working on support for WebSockets.

	- Fixed some compiler warnings when compiling with -Wextra

	- Thanks to Jan Jaeger's excellent bug report, made some changes
	that should make it easier to build ShellInABox for OpenWRT.

## 2009-12-10  Markus Gutschke  <markus@shellinabox.com>

	- Add .note.GNU-stack to all object files so that the generated
	binary doesn't erroneously request an executable stack.

## 2009-12-03  Markus Gutschke  <markus@shellinabox.com>

	- Allow retrieval of the user's default login shell from
	/etc/passwd.

	- Allow the code to be built without support for the LOGIN
	service, as calling /bin/login does not work well on Fedora.

## 2009-12-02  Markus Gutschke  <markus@shellinabox.com>

	- Added fallback code that dynamically computes the correct commandline
	arguments for "objcopy" if building for an otherwise unknown target
	platform.

## 2009-12-01  Markus Gutschke  <markus@shellinabox.com>

	- Added some basic sanity checks to the commit script that now makes
	sure we at least attempt to keep copyright dates updated whenever we
	make changes.

	- Added checks that the debian/changelog file is up-to-date

	- Added debian/watch file

	- Updated the Standards-Version in debian/control. Still need to
	review whether we are in full compliance, though.

	- Fixed lintian errors.

## 2009-11-29  Markus Gutschke  <markus@shellinabox.com>

	- Preparations for packaging ShellInABox in a way that makes it
	easy for Debian package maintainers to pick it up.

## 2009-11-25  Markus Gutschke  <markus@shellinabox.com>

	- On browsers that support CSS transforms, enable switching between
	  80 and 132 column mode.

## 2009-11-21  Markus Gutschke  <markus@shellinabox.com>

	- Updated manual page documenting --user-css

	- Released version 2.10

## 2009-11-18  Markus Gutschke  <markus@shellinabox.com>

	- Fixed some compiler warnings when using more recent versions of
	gcc and glibc.

	- Tweak the handling of CTRL keys, so that some of the more unusual
	combinations work. For historic reasons, there is an expectation that
	CTRL-3..CTRL-8 return specific control characters. Also fixed the
	handling of CTRL-\ which could cause problems with some browsers.

	- Rely on the browser for capitalization. This should fix Capslock
	behavior. Hopefully, it won't break any other keyboard features or
	layouts.

## 2009-08-20  Markus Gutschke  <markus@shellinabox.com>

	- Added transparent printing support. The development of this
	feature is sponsored by De Bortoli Wines Pty Limited and by
	Eternity Technologies.

## 2009-08-19  Markus Gutschke  <markus@shellinabox.com>

	- Added a ${url} parameter that can be used in the service description.

## 2009-08-11  Markus Gutschke  <markus@shellinabox.com>

	- Added support for user selectable style sheets. Included example
	style sheets that allow switching to white-on-black or to monochrome
	mode from the right click context menu.

	- Fixed the "|" key on Swedish keyboards.

## 2009-07-30  Markus Gutschke  <markus@shellinabox.com>

	- Added the --css command line option to make incremental changes
	to the style sheet without having to load a full replacement with
	the --static-file option. Added an example that enables white text
	on a black background.

	- Added Debian specific documentation to the manual page.

## 2009-07-29  Markus Gutschke  <markus@shellinabox.com>

	- Allow unprivileged users to run the daemon. This requires
	calling "ssh" instead of "login".

## 2009-07-27  Markus Gutschke  <markus@shellinabox.com>

	- Use JavaScript redirection for attaching the missing slash to
	the URL. This should make it easier to use reverse proxies. It was
	already possible to run shellinaboxd behind a proxy, but a lot of
	users got the configuration wrong.

## 2009-07-08  Markus Gutschke  <markus@shellinabox.com>

	- Optionally compress large responses, if the browser accepts
	deflate compression. This mainly improves start up time.

	- More fine tuning of the regular expressions that detect URLs.
	We now allow '.' and ',' in URLs, as long as they are not at the
	very end of the URL, where they would probably be part of the
	enclosing sentence and not actually part of the URL.

## 2009-07-06  Markus Gutschke  <markus@shellinabox.com>

	- Making it easier to host the terminal on non-root URLs by always
	redirecting to a URL that includes a trailing slash.

	- Run-time testing for availability of libpthread functions does not
	work reliably on some platforms. So, avoid doing so on anything
	other than Linux/i386. For all other platforms, assume that the code
	is not linked against libpthread. For ShellInABox, this is always
	the correct assumption. But if the code gets embedded into other
	projects, this might have to be changed.

## 2009-07-05  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.9

## 2009-07-04  Markus Gutschke  <markus@shellinabox.com>

	- Refined regular expressions for finding URLs.

	- Show new terminal size when resizing the browser.

	- Restored compatibility with IE5 and IE6.

## 2009-07-03  Markus Gutschke  <markus@shellinabox.com>

	- Added --linkify option. Default settings cause the terminal to
	recognize fully qualified URLs and to make them clickable.

## 2009-06-28  Markus Gutschke  <markus@shellinabox.com>

	- Added support for keyboards that have a dedicated "<" / ">" key.

## 2009-06-21  Markus Gutschke  <markus@shellinabox.com>

	- Added --localhost option.

	- Added support for building on ARM.

	- Respect "Connection: close" for proxies that rely on pre-HTTP/1.1
	behavior.

## 2009-05-24  Markus Gutschke  <markus@shellinabox.com>

	- Added SSL support for OpenBSD

## 2009-05-23  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.8

## 2009-05-22  Markus Gutschke  <markus@shellinabox.com>

	- Improved support for entering non-ASCII characters.

## 2009-05-20  Markus Gutschke  <markus@shellinabox.com>

	- Fixed various issues with building on OpenBSD

## 2009-04-28  Markus Gutschke  <markus@shellinabox.com>

	- Fixed variable expansion in service descriptions.
	
## 2009-04-27  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.7

	- Improved compatibility with some PAM configurations when running
	as a non-privileged user.

	- Fixed a bug that required shells to output data (e.g. a prompt)
	before they could read the first data.

	- Fixed a potential crash.

## 2009-04-12  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.6

	- The demo application is still incomplete, but starting to be
	somewhat functional. The BASIC interpreter supports variables, and
	can parse expressions. But it is still missing all flow-control
	commands, making it somewhat useless for writing real programs.

## 2009-03-30  Markus Gutschke  <markus@shellinabox.com>

	- Added initial revision of demo application.

	- Show fatal error message even when running in "quiet" mode.

	- Make it easier to override parameters needed by the system startup
	scripts.

## 2009-03-29  Markus Gutschke  <markus@shellinabox.com>

	- Added support for chained SSL certificates

## 2009-03-23  Markus Gutschke  <markus@shellinabox.com>

	- Added an INSTALL.Debian file with Debian-specific instructions on
	how to build and install a package file.

## 2009-03-21  Markus Gutschke  <markus@shellinabox.com>

	- Possible fix for IE problems with horizontal positioning of
	cursor if the line ends in spaces.

	- Work-around for an IE6 bug when doing HTTPS through proxies.
	
## 2009-03-21  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.5

	- More testing on older IE versions.

## 2009-03-19  Markus Gutschke  <markus@shellinabox.com>

	- Fixed cursor positioning. Hopefully, more browsers will be happy
	with this, now.

	- Explicitly added no-cache headers to our responses. This might help
	with the IE6 problems.

## 2009-03-17  Markus Gutschke  <markus@shellinabox.com>

	- Allow root to bind to privileged port.

## 2009-03-17  Markus Gutschke  <markus@shellinabox.com>

	- Fixed IE6 support.

	- Fixed possible memory corruption, when sessions time out.

## 2009-03-16  Markus Gutschke  <markus@shellinabox.com>

	- Fixed some compiler warnings, that newer versions of GCC issue.

## 2009-02-27  Markus Gutschke  <markus@shellinabox.com>

	- Added fallback on old-style pty's, if /dev/pts is not mounted.

	- Work-around for systems that don't define a "nogroup" group.

	- Remove the dependency on fdopendir, which does not exist
	everywhere.

## 2009-02-16  Markus Gutschke  <markus@shellinabox.com>

	- Include VCS revision number in user-visible version string.

	- Allow "configure" to select whether OpenSSL and PAM libraries
	should be used at all, dynamically searched-for at run-time, or
	linked as a regular dynamic library.

	- Fixed various bugs that prevents ShellInABox from running on
	FreeBSD

## 2009-02-12  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.4

## 2009-02-11  Markus Gutschke  <markus@shellinabox.com>

	- Fixed fatal compiler warning if compiling without SSL support.

	- Fixed cursor hiding and showing

	- Fixed various rendering glitches reported by Phil Endecott of
	Anyterm (http://anyterm.org) fame.

	- Made code more portable. In particular, fixed sed scripts.

	- Added explicit config.h file, instead of passing configuration
	options on the compiler's command line.

	- Fixed compilation issues on BSD systems. Code is still untested
	and unsupported on non-Linux systems at this time.

## 2009-01-21  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.3

	- Fixed a show-stopper bug that broke the --cert option.

## 2009-01-21  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.2

	- Fixed a bug that could result in the font getting corrupted.

	- Improved compatibility with more versions of the OpenSSL library.
	Previously, the feature test for TLSEXT did not always work correctly,
	resulting in compilation failures.

	- Improved support for embedding shellinaboxd into existing web
	services. SSL certificates can now be passed in through a file
	handle, and port and pid numbers can be retrieved from the CGI header.

## 2009-01-08  Markus Gutschke  <markus@shellinabox.com>

	- Released version 2.1

	- Fixed build errors mostly related to x86_64.

	- Added --no-beep command line option to avoid VLC plugin crashing
	Firefox/x86_64.

	- Fixed multi-line selections in Firefox.

## 2009-01-01  Markus Gutschke  <markus@shellinabox.com>

	- Added CGI mode for demand-loading the shellinaboxd daemon
	from a web server. This also allows for the web server to
	perform authentication, instead of having shellinaboxd do so.
	
	- Tightened setuid-root operation to no longer allow switching
	to arbitrary users/groups. As before, setuid-root remains a
	non-standard configuration that is not currently recommended.
	
	- Fixed session management to deal better with torn down
	connections. Closed one bug that could have resulted in
	permanently orphaned connections, when the browser navigated
	away from the page.

## 2008-12-27  Markus Gutschke  <markus@shellinabox.com>

	- First public release of the version 2.0 rewrite. This is the
	first release of ShellInABox that supports an AJAX interface
	instead of the original Java applet.