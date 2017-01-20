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

Note that many of these MIB's have been curated to fix encoding errors
or other similar problems.

Each directory is used for one vendor.  To actually use this with
most software, you'll have to put the MIB's you want all into a single
directory and point the software at that.  Note that actually loading
everything at the same time may not work as you expect.

The following vendors are represented here:
* Cisco: Huge number of MIB's, some of which don't exactly work with
  standards compliant tools.  Obtained directly from Cisco using
  snmp-mibs-downloader from Debian.
* Fraunhofer FOKUS: These are the custom MIB's used on many BSD systems.
  If you are monitoring FreeNAS or pfSense systems, you want these.
  Obtained from the FreeBSD sources and a couple of network monitoring
  tools whose names I don't recall.
* IANA: Most of these are just numerical registries, some are used by
  other MIB's.  Obtained directly from the IANA site.
* IEEE: All the 802.x related MIB's I could find.  These all
  relate to network switches and similar devices.  Obtained directly
  from the IEEE site, then curated to fix the smart quotes and bad line
  endings throughout them.
* IETF: All the RFC MIB's. At least some of these are needed no matter
  what, most are optional though.  Obtained directly from the IETF site.
* IRTF: Some network manaement research group related stuff.  Obtained
  from the Gentoo distribution of libSMI.
* Jacobs University Brenen: Mostly of interest for monitoring sensor
  networks.  Obtained from the Gentoo distribution of libSMI.
* Juniper: JunoS and ScreenOS related MIB's.  Obtained directly from
  Juniper using snmp-mibs-downloader from Debian.
* Microsoft: A handful of Windows MIB's.  The only ones likely to be of
  significant interest are MSFT, WINS, and WINDOWS-NT-PERFORMANCE.
  Obtained from various sources online, then curated to fix encoding
  and naming issues.
* TU Braunschweig: General monitoring stuff for Linux and Xen.  I know of
  nothing that actually implements these, but they're part of the standard
  libsmi install.  Obtained from the Gentoo distribution of libSMI.
* UC Davis: General purpose system monitoring.  Almost every UNIX-like
  system with SNMP support implements at least a subset of these.
  Includes the LM-SENSORS MIB as well.  Mostly obtained from Net-SNMP.
* University of Deleware: Contains some NTP related MIB's.  Found in
  multiple network monitoring tool's sources.
