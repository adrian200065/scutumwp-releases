# ScutumWP releases

Built, signed release packages of the ScutumWP Security WordPress plugin.
Installed copies of the plugin check this repository's latest release for
updates through WordPress's normal update screen.

Every release includes `update.json`, which carries an Ed25519 signature over
`scutumwp|<version>|<sha256 of the zip>`. The plugin refuses to install any
package whose signature doesn't verify against the public key compiled into it,
so a modified or relabelled zip is rejected even if it is uploaded here.

Source code is not published in this repository.
