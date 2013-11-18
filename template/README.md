# Plack/PSGI Perl application

## Structure

- app.psgi : Your PSGI application.
- cpanfile : Lists CPAN modules that your application depends on.
- lib/     : Your Perl module library. lib/ is automatically prepended to
             PERL5LIB environment variable.
- t/       : Directory your test scripts reside. *.t files are executed by
             "prove" command. Nested directories are searched recursively.
