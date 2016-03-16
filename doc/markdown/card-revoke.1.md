NAME
====

**card-revoke** -- revoke Card from the Public Keys Service

SYNOPSIS
========

**virgil card-revoke** {-f *file*|-d *arg*} -a *arg* -k *file* \[--\]
\[--version\] \[-h\]

DESCRIPTION
===========

Revoke a Card from the Public Keys Service

OPTIONS
=======

    -f *file*,  --validated-identities *file*
     (OR required)  Validated identity
         -- OR --
    -d *arg*,  --identity *arg*
     (OR required)  Identity user


    -a *arg*,  --card-id *arg*
     (required)  Virgil Card identifier

    -k *file*,  --key *file*
     (required)  Private key

    --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag

    --version
     Displays version information and exits

    -h,  --help
     Displays usage information and exits

EXAMPLES
========

1.  Revoke Virgil Card with a confirmed identity:

        virgil card-revoke -a *card_id* -f *validated-identities.txt -k private.key

2.  Revoke Virgil Card with a confirmed identity:

        virgil card-revoke -a *card_id* -d email:user@domain.com -k private.key

SEE ALSO
========

[`virgil(1)`]()  
[`card-create(1)`]()  
[`public-key-revoke(1)`]()