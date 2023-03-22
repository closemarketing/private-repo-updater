# Private Repositories Plugin Updater
Library to update plugins from GitHub repositories.

## Usage
```
if ( is_admin() ) {
  include_once plugin_dir_path( __FILE__ ) . '/class-wp-private-updater.php';
	$config  = array(
		'github_uri' => 'https://api.github.com/repos/fgrweb/pontewordcamp/releases',
		'token'      => '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',
	);
	$updater = new Ponte_WordCamp_Updater( $config, __FILE__ );
	$updater->fgr_check_update();
}
```
