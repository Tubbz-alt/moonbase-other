EDITOR=`which $EDITOR 2>/dev/null` ||
EDITOR=`which nano` &&

OPTS+=" --enable-tmpfiles.d \
        --with-editor=$EDITOR \
        --with-rundir=/run/sudo \
        --with-vardir=/var/db/sudo \
        --with-sendmail=/usr/bin/sendmail"

OPTS+=" --sbindir=/usr/bin"

default_build
