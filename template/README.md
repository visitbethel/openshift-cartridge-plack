# Plack/PSGI Perl application

## Structure

- app.psgi :
  Your PSGI application.
  
- cpanfile :
  List of CPAN modules that your application depends on.
  
- env.pl :
  Script to set environment variables to control how "plackup" should work.
  
- lib/ :
  Your Perl module library. lib/ is automatically prepended to
  PERL5LIB environment variable.
  
- t/ :
  Directory your test scripts reside. *.t files are executed by
  "prove" command.
  
- .proverc :
  Options for "prove" command.


## Environment Variables

- OPENSHIFT_PLACK_LOG_DIR :
  Directory path in which you should store your log files. It is up to
  you to write and rotate logs in this directory. The log files are
  cleaned up by "tidy" command.
