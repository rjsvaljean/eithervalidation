EitherValidation
================
This is a single file approach to treating Scala's standard library Either class
like a Scalaz validation. It provides a mechanism for treating Either as an
applicative functor by enriching it with an #apply method when the Right type
is a function.

Please see EitherValidation and EitherValidationSpec for more details. This
is a work in progress.

Instructions
============

 1. Install `sbt`, -OR- create a symlink to the `sbt` installed as part of `play`

        # I have this as ~/bin/sbt, and the ~/bin directory is in my PATH
        SBT_DIR="/opt/play/framework/sbt"
        java -Xms512M -Xmx1536M -Xss1M -XX:+CMSClassUnloadingEnabled -XX:MaxPermSize=384M -jar $SBT_DIR/sbt-launch.jar "$@"

 2. Run tests

        sbt test

 3. Generate IntelliJ project

        sbt gen-idea
