# StopForumSpam.com - PHP Lib

A PHP wrapper class for the API available at [stopforumspam.com](http://www.stopforumspam.com/usage). An API key is required only for updating the spam database. Uses the JSON interface internally.

## Examples

### Check if user has been recorded as a spammer

	$sfs = new StopForumSpam();
	$args = array('email' => 'email@example.com', 'ip' => '192.168.1.1', 'username' => 'JohnDoe');
	$spamcheck = $sfs->is_spammer( $args );

### Get datailed data for suspected spammer

This is the data, as returned by StopForumSpam.com, without parsing.

	$sfs = new StopForumSpam();
	$args = array('email' => 'email@example.com', 'ip' => '192.168.1.1', 'username' => 'JohnDoe');
	$user = $sfs->get( $args );

## License

Licensend under the [BSD 3-Clause License](http://www.opensource.org/licenses/BSD-3-Clause).