NAME
====

**verify** -- verify data.

SYNOPSIS
========

**virgil verify** [--in *file*] [--out *file*] --sign *file*
--sign-owner *arg*

DESCRIPTION
===========

Verify data with given user's identifier or with it Virgil Public Key.

OPTIONS
=======

-i *file*, --in *file*  
Data to be verified. If omitted stdin is used.

-o *file*, --out *file*  
Verification result: `success` | `failure`. If omitted stdout is used.

-s *file*, --sign *file*  
(required) Digest sign.

-r *arg*, --sign-owner *arg*  
(required) Sign owner, defined in format:

    [file|email|phone|domain]:<value>

where:

-   if `file`, then *value* - signers's Virgil Public Key file stored
    locally;
-   if `email`, then *value* - signers's email;
-   if `phone`, then *value* - signers's phone;
-   if `domain`, then *value* - signers's domain.

SEE ALSO
========

`virgil(1)`, `virgilsign(1)`