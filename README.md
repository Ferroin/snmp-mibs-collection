# snmp-mibs-collection #
This is a collection of MIB's for use with SNMP management tools.
It's by no means an exhaustive collection, but it does cover most of
the more common systems.  This constitutes what I personally consider
a basic set given typical network infrastructure.  It includes all the
current IETF and IANA MIB's, as well as an assortment of vendor MIB's
that cover most common systems.

This whole thing originated because of how much effort I had to put into
getting just the basic set of MIB's for managing Windows.  I couldn't
find a single site that both worked and allowed bulk download of all
the MIB's they provided.  As a result of this, I started this collection
so I wouldn't have to deal with that crap again.

Each directory is used for one vendor.  To actually use this with
most software, you'll have to put the MIB's you want all into a single
directory and point the software at that.  Note that actually loading
everything at the same time may not work as you expect.
