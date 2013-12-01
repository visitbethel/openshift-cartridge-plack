
# OpenShift cartridge for Plack/PSGI Perl applications

This is a Web application cartridge based on Plack/PSGI for
OpenShift. PSGI is an interface specification for Web applications
written in Perl, and Plack is a PSGI toolkit implementation.

The big difference from the `perl` cartridge (officially supported by
OpenShift team) is that the Plack cartridge allows you to run any PSGI
server while `perl` cartridge is limited to Apache HTTPD + mod_perl
configuration.


# How to Use

First, create your app with the stable release.

    $ rhc create-app -a YOUR_APP_NAME -t https://raw.github.com/debug-ito/openshift-cartridge-plack/tree/0.0.1/metadata/manifest.yml

Do not use the master branch because it may be broken when I'm
debugging something.

Then, edit `app.psgi` created in `YOUR_APP_NAME` directory, commit the
change and `git push` it. The PSGI application is executed in the
cloud.

See README.md created in `YOUR_APP_NAME` directory for further details.


# Acknowledgement

* perl http://www.perl.org/
* Plack/PSGI http://plackperl.org/
* App::cpanminus https://metacpan.org/pod/App::cpanminus
* Daemon::Control https://metacpan.org/pod/Daemon::Control
* bin/setup script is inspired from heroku-buildpack-perl.
  https://github.com/miyagawa/heroku-buildpack-perl/blob/master/bin/compile


# Author

* Toshio Ito - https://metacpan.org/author/TOSHIOITO

