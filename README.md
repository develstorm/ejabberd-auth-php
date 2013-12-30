## ABOUT

This is a collection of bridges allowing an ejabberd XMPP server to use a locally installed PHP-based CMS for external authentication.

## FEATURES

Currently implemented bridges:

* phpBB 3.0
* phpBB 3.1 (unstable)
* Drupal 7.x
* Drupal 8.x (unstable)

Potential candidates for further bridges are WordPress, MediaWiki, Joomla! and Moodle.

## EXTENDING

In order to create a new plugin named <xyz>, you will need the following:

* A class extending EjabberdAuthBridge and implementing its methods.
* A file named <xyz>.module that contains the function <xyz>_init().
* <xyz>_init() will receive its appropriate conf array in config.php.
* <xyz>_init() must return an instance of the extended class.

## LICENSE

The core project, without plugins, is available under the terms of the GNU General Public License, version 2 or later.

Plugins are individually licensed:

* phpBB, all versions: GNU General Public License, v2
* Drupal, all versions: GNU General Public License, v2 and later.

GPL v2: http://www.gnu.org/licenses/gpl-2.0.txt
GPL v3: http://www.gnu.org/licenses/gpl-3.0.txt