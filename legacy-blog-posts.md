# Legacy Blog Posts

From 2011-2019, a series of blog posts related to the BitCurator projects were published to **https://bitcurator.net**. Those posts have been replicated here for reference.

* [2019 Posts](#2019-posts)
* [2018 Posts](#2018-posts)
* [2017 Posts](#2017-posts)
* [2016 Posts](#2016-posts)
* [2015 Posts](#2015-posts)
* [2014 Posts](#2014-posts)
* [2013 Posts](#2013-posts)
* [2012 Posts](#2012-posts)
* [2011 Posts](#2011-posts)

## 2019 Posts

### Latest Release(s) (originally published January 3, 2019)

Looking for the latest release of the BitCurator environment? You can find it at [https://github.com/BitCurator/bitcurator-distro/wiki/Releases](https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

Looking for other tools produced by the BitCurator team? You can find an overview at [https://bitcurator.github.io/](https://bitcurator.github.io).

## 2018 Posts

### BitCurator 2.0.10 Released (originally published December 14, 2018)

A new production release of BitCurator (2.0.10) is now available at the BitCurator release portal.

You can download the VirtualBox VM and installation ISO directly using the following links:

[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.10.tar.gz](http://distro.ibiblio.org/bitcurator/BitCurator.2.0.10.tar.gz)
[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.10.iso](http://distro.ibiblio.org/bitcurator/BitCurator-2.0.10.iso)

BitCurator 2.0.10 is a maintenance release. It includes package and kernel updates in the core OS, restores the ficlam script to the expected location for the bcadmin user, and adds a command line reference sheet to the documentation.

Questions? Visit the [BitCurator Users Group](https://groups.google.com/forum/#!forum/bitcurator-users) to speak with members of the community.

### BitCurator 2.0.8 released (originally published November 13, 2018)

A new production release of BitCurator (2.0.8) is now available at [the BitCurator release portal](https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

You can download the VirtualBox VM and installation ISO directly using the following links:

[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.8.tar.gz](http://distro.ibiblio.org/bitcurator/BitCurator.2.0.8.tar.gz)
[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.8.iso](http://distro.ibiblio.org/bitcurator/BitCurator-2.0.8.iso)

BitCurator 2.0.8 is a maintenance release that updates Sleuthkit to 4.6.4, preloads VirtualBox 5.2.22 guest additions in the VM, and includes various package updates in the core OS.

Questions? Visit the [BitCurator Users Group](https://groups.google.com/forum/#!forum/bitcurator-users) to speak with members of the community.

### BitCurator 2.0.6 released (originally published August 7, 2018)

A new production release of BitCurator (2.0.6) is now available at [the BitCurator release portal](https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

You can download the VirtualBox VM and installation ISO directly using the following links:

[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.6.tar.gz](http://distro.ibiblio.org/bitcurator/BitCurator.2.0.0.tar.gz)
[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.6.iso](http://distro.ibiblio.org/bitcurator/BitCurator-2.0.0.iso)

BitCurator 2.0.6 fixes several long-standing issues related to environment stability when the environment is installed as a host operating system on single or multi-boot systems.

A couple of the most commonly reported issues with previous BitCurator releases (when installed as a host OS) have been (a) failure to recognize or mount the host OS drive after reboot with read-only enforcement enabled, and (b) the unintuitive/fragile process required to permanently write-enable specific drives installed in the machine other than the boot disk  – drives that are typically used for secondary or working storage.

These issues are addressed in the 2.0.6 release as follows:

* Fixed a bug in rbfstab that in some cases caused the contents of the file system mount record (fstab) to be lost on reboot due to automatic cleaning of a temporary directory used by rbfstab, and resulting in a black screen (failure to boot to the desktop). In 2.0.6, read-only enforcement remains off by default, but may be enabled and left enabled between reboots after installation.
* Updated the read-only enforcement tool (rbfstab) to target only USB devices. Secondary storage devices permanently mounted in the host system will no longer be affected, and multi-boot systems (e.g. BitCurator/Windows dual-boot) should now remain stable between reboots. Dialog text for the mount-policy appindicator on the desktop (the red/green disk icon) has been updated to reflect this change. Drive automounting remains disabled in all states, as with previous releases.

VirtualBox 5.2.16 guest additions are preloaded in the 2.0.6 VM.

Need to find an older 16.04LTS-based release? You can find available releases in the “Release Notes” section of the BitCurator release portal.

Questions? Visit the BitCurator Users Group to speak with members of the community.

### BitCurator 2.0.0 released (originally published July 20, 2018)

A new production release of BitCurator (2.0.0) is now available at the BitCurator release portal.

You can download the VirtualBox VM and installation ISO directly using the following links:

[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.0.tar.gz](http://distro.ibiblio.org/bitcurator/BitCurator.2.0.0.tar.gz)
[http://distro.ibiblio.org/bitcurator/BitCurator-2.0.0.iso](http://distro.ibiblio.org/bitcurator/BitCurator-2.0.0.iso)

BitCurator 2.0.0 is the first official Ubuntu 18.04LTS-based release of BitCurator.

* Desktop performance in the VM significantly improved
* Various security and power management updates for modern hardware
* Read-only mount protection for all non-boot devices is disabled by default to reduce commonly reported boot failure issues on installed systems. RO mount protection may still be enabled by selecting the mount status icon in the indicator menu (as in previous releases), but should not be left enabled between boots. Use with caution, or use a hardware write blocker!
* Attached devices are no longer displayed in the dock (default behavior in Ubuntu 18.04LTS). Since automount remains disabled in BitCurator 2.0.0, you must open a file browser (click “Files” icon in the dock) to view attached devices.

VirtualBox 5.2.16 guest additions are preloaded in the 2.0.0 VM.

Need to find an older 16.04LTS-based release? You can find available releases in the “Release Notes” section of [the BitCurator release portal](https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

Questions? Visit the [BitCurator Users Group](https://groups.google.com/forum/#!forum/bitcurator-users) to speak with members of the community.

### BitCurator 1.8.22 released (+ early preview of BitCurator 2.0.0) (originally published April 17, 2018)


A new production release of BitCurator (1.8.22) is now available at [the BitCurator release portal](https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

You can download the installation ISO and preconfigured VM directly using the following links:

[http://distro.ibiblio.org/bitcurator/BitCurator-1.8.22.iso](http://distro.ibiblio.org/bitcurator/BitCurator-1.8.22.iso)
[http://distro.ibiblio.org/bitcurator/BitCurator-1.8.22.tar.gz](http://distro.ibiblio.org/bitcurator/BitCurator-1.8.22.tar.gz)

This is a maintenance release, and includes an updated Linux kernel, VirtualBox 5.2.8 guest additions, and other support software library updates.

Interested in testing out an upcoming release? Visit our revised download landing page at:

[https://github.com/BitCurator/bitcurator-distro/wiki/Releases](https://github.com/BitCurator/bitcurator-distro/wiki/Releases)

and scroll down to “Release Notes” for links to an early beta release of BitCurator 2.0.0. BitCurator 2.0.0 will be the first release of BitCurator based on Ubuntu 18.04LTS. Stay tuned to the [BitCurator Users Group](https://groups.google.com/forum/#!forum/bitcurator-users) for more information on this release in the coming weeks.

### Registration for nlp4arc 2018 is now open (originally published January 5, 2018)

We are pleased to announce that registration for the BitCurator NLP Forum 2018 (nlp4arc) is now open. The event will focus on the application of natural language processing (NLP) to support use, access, and analysis of digital primary source materials. [Click here to register](https://apps.research.unc.edu//events/index.cfm?event=events.eventDetails&event_key=F8EA6B9CFF725F243F3B10CD8972FEC189017DD6).

A rapidly growing body of materials with significant cultural value are “born digital.” Information professionals must be prepared to extract digital materials from their original environments and media in ways that reflect the rich metadata and ensure the integrity of the materials. They must also support new forms of access: allowing users to make sense of materials and understand their context.

There are many types of contextual information that can be vital to making sense and meaningful use of digital objects. These can include objects, agents, occurrences, purposes, times, places, form of expressions, concepts/abstractions and relationships.

There are many existing open-source tools that libraries, archives and museums (LAMs) can use to identify, extract and expose such contextual entities from the wide diversity of born-digital materials that LAMs already hold and continue to receive. NLP tools and methods can help to both (1) facilitate curatorial decision making and description, and (2) generate access points to be presented to end users.

nlp4arc 2018
February 2, 2018 – 9:00am – 5:00pm Dey Hall, Toy Lounge
University of North Carolina
Chapel Hill, North Carolina
Suggested hashtag: #nlp4arc

**Program**

|:|:
|9:00-9:15|Welcome and introduction – Cal Lee|
|9:15-10:30|Foundations and Strategies
Michael Piotrowski, University of Lausanne – Historical Texts, NLP, and Formal Models
Daniel Pitti, University of Virginia – Name Entities, Named Entities, Facts in Contexts
Carl Wilson, Open Preservation Foundation – Not Just Building Tools: Strategies for Sustaining Software and Associated Communities
Mark Matienzo, Stanford University – Practical and Ethical Considerations of NLP Applied to Humanitarian Digital Libraries|
|10:30-10:45|Break|
|10:45-12:00|Implementation and Projects
Mary Elings, University of California, Berkeley – Using NLP to Support Dynamic Arrangement, Description, and Discovery of Born Digital Collections
Jeremy Gibson and Nitin Arora, North Carolina Department of Natural and Cultural Resources – “Honey, I Tagged the Email! Now What?”: NLP and the TOMES Project
Ryan Shaw, University of North Carolina at Chapel Hill – Gathering Specimens to Augment Authority Files
Stéfan Sinclair, McGill University – Spyral Notebooks: Some Reasons Why the World Needs Yet Another Jupyter|
|12:00-12:30|Panel on NLP Lessons Learned
Jaime Arguello, University of North Carolina at Chapel Hill
Stephanie Haas, University of North Carolina at Chapel Hill|
|12:30-1:30|Lunch|
|1:30-2:15|Enabling Technologies
Laney McGlohon, ArchiveSpace – Finding the Data: The Use of a Data
Dictionary in Retrieving Descriptive Metadata from ArchivesSpace
Kam Woods and Cal Lee, University of North Carolina at Chapel Hill – BitCurator NLP Development and Plans|
|2:15-2:45|Generation of Breakout Topics|
|2:45-3:00|Break|
|3:00-3:45|Breakout Sessions|
|3:45-4:15|Reporting Back from Breakout Sessions|
|4:15-5:00|Wrap Up and Next Steps|

**Registration**
General Registration – $30
Student & BitCurator Consortium Members Registration – $15
Register [here](https://apps.research.unc.edu//events/index.cfm?event=events.eventDetails&event_key=F8EA6B9CFF725F243F3B10CD8972FEC189017DD6).

**Accommodations**
Please see the list of nearby hotels below.

The Carolina Inn 211 Pittsboro Street
Chapel Hill, NC 27516
Tel 800.962.8519
(This is the closest option. It is on the UNC Campus, just a couple of blocks from the Student Union.)

Hampton Inn & Suites Chapel Hill Carrboro/Downtown
370 East Main Street, Unit 100
Carrboro, North Carolina 27510
Tel 919.969.6988
(Walkable distance)

Holiday Inn Express Chapel Hill
6119 Farrington Road
Chapel Hill, NC 27517
Tel 919.489.7555

Aloft Chapel Hill
1001 South Hamilton Road
Chapel Hill, NC 27517
Tel 866.716.8143
(Shuttle buses available)

## 2016 Posts

### Registration for nlp4arc is now open (originally published December 13, 2016)

We are pleased to announce that registration for the BitCurator NLP Forum 2017 (nlp4arc) is now open. The event will focus on the application of natural language processing (NLP) to support use, access, and analysis of digital primary source materials. Click [here](https://apps.research.unc.edu//events/index.cfm?event=events.eventDetails&event_key=C74093AEB6E043701179590C9D87F79BCBF73379) to register.

A rapidly growing body of materials with significant cultural value are “born digital.” Information professionals must be prepared to extract digital materials from their original environments and media in ways that reflect the rich metadata and ensure the integrity of the materials. They must also support new forms of access: allowing users to make sense of materials and understand their context.

There are many types of contextual information that can be vital to making sense and meaningful use of digital objects. These can include objects, agents, occurrences, purposes, times, places, form of expressions, concepts/abstractions and relationships.

There are many existing open-source tools that libraries, archives and museums (LAMs) can use to identify, extract and expose such contextual entities from the wide diversity of born-digital materials that LAMs already hold and continue to receive. NLP tools and methods can help to both (1) facilitate curatorial decision making and description, and (2) generate access points to be presented to end users.

The day will include a series of short talks by internationally-recognized experts, followed by a set of participant-driven unconference discussions. Speakers will include:

* Christopher (Cal) Lee (PI), University of North Carolina at Chapel Hill
* Kam Woods (Co-PI, Technical Lead), University of North Carolina at Chapel Hill
* Mary Elings, University of California, Berkeley
* Don Mennerich, New York University
* Daniel Pitti, University of Virginia
* Josh Schneider, Stanford University
* Ryan Shaw, University of North Carolina at Chapel Hill
* Brad Westbrook, ArchivesSpace
* Carl Wilson, Open Preservation Foundation
* Hugh Cayless, Duke University Libraries
* Jeremy Gibson, North Carolina Department of Natural and Cultural Resources

**Event Information**
Date: 3 February 2017 9:00am – 5:00pm
Location: Student Union rooms 3206A and 3206B, University of North Carolina, Chapel Hill, North Carolina

**Registration**
General Registration – $30
Student & BitCurator Consortium Members Registration – $15
Register [here](https://apps.research.unc.edu//events/index.cfm?event=events.eventDetails&event_key=C74093AEB6E043701179590C9D87F79BCBF73379).

Accommodations
Please see the list of nearby hotels below.

The Carolina Inn 211 Pittsboro Street
Chapel Hill, NC 27516
Tel 800.962.8519
(This is the closest option. It is on the UNC Campus, just a couple of blocks from the Student Union.)

Hampton Inn & Suites Chapel Hill Carrboro/Downtown
370 East Main Street, Unit 100
Carrboro, North Carolina 27510
Tel 919.969.6988
(Walkable distance)

Holiday Inn Express Chapel Hill
6119 Farrington Road
Chapel Hill, NC 27517
Tel 919.489.7555

Aloft Chapel Hill
1001 South Hamilton Road
Chapel Hill, NC 27517
Tel 866.716.8143
(Shuttle buses available)

### BitCurator NLP Announced! (originally published October 17, 2016)

The University of North Carolina at Chapel Hill has received a grant for $750,000 from the Andrew W. Mellon Foundation to support BitCurator NLP, a project that will develop software and protocols for the application of natural language processing (NLP) methods to born-digital library, archives and museum (LAM) collections.

See the [full press release](https://sils.unc.edu/news/2016/bitcurator-nlp) on the UNC SILS site.

### Looking for the latest? (originally published June 23, 2016)

Visit the [BitCurator Consortium page](https://www.bitcuratorconsortium.org/) for the latest news!

### CurateGear + BUF 2016 Wrap Up! (originally published January 18, 2016)

Thanks to everyone who attended and/or participated in CurateGear and the BitCurator Users Forum!

CurateGear 2016 was an interactive day-long event focused on digital curation tools and methods. Participants saw demonstrations, heard about the latest developments, and discussed application in professional contexts. The event was sponsored by the School of Information and Library Science at the University of North Carolina at Chapel Hill and the Andrew W. Mellon Foundation (through the BitCurator Access project).

Presentation slides for CurateGear are now available [here](http://ils.unc.edu/digccurr/curategear2016.html).
Abridged notes from each presentation can be found [here](http://ils.unc.edu/digccurr/curategear2016-notes.pdf).

We’ll be posting more BUF wrap up soon – stay tuned! In the meantime, check out the [twitter feed from the event](https://twitter.com/hashtag/buf2016?src=hash).

## 2015 Posts

### Program + registration available for the BitCurator Users Forum 2016 (originally published December 4, 2015)

We are pleased to announce the preliminary program is now available for the BitCurator Users Forum 2016. The Forum takes place the day after [CurateGear 2016](http://ils.unc.edu/digccurr/curategear2016.html).

Join BitCurator users from around the globe as we discuss how we are using the BitCurator software environment. Hosted by the BitCurator Consortium (BCC), this event will be grounded in the practical, real-world experiences of digital archivists and digital curation experts. Come prepared to discuss your current challenges, share emerging BitCurator integrations and workflows, and address the “now what” of handling your digital forensics outputs.

Date: 15 January 2016
Location: Pleasants Family Assembly Room, Wilson Library, University of North Carolina, Chapel Hill, North Carolina

Registration
General Registration – $30
Student Registration – $15
BitCurator Consortium Member Registration – Free
Register [here](https://bitcuratorconsortium.org/events/buf2016/registration).

Program
8:00 – 8:30am Registration and Coffee
8:30 – 9:00am Welcome and Introductions
9:00 – 10:15am Panel: Beyond Floppy Disks
Cultural heritage institutions are collecting a larger variety of media than ever before including external hard drives, computers, and files from hosted cloud services. While there are established workflows and best practices for smaller media objects, many institutions are just now beginning to tackle these other forms of media.

This panel will be a forum to discuss how some institutions are ingesting files from various media types, including the utilization of new tools and the development of new policies and workflows.
10:15 – 10:45am Break
10:45 – 12:00pm Lightning Talks: Not Your Average BitCurator: How Repositories are Using BitCurator Tools in Different Ways
As institutions become exposed to alternative digital forensic tools and their individual strengths and limitations, they are exploring the benefits of expanding their digital curation toolset beyond reliance on any single product. Moreover, the modular architecture of tools like BitCurator has fostered a growing community of contributors who have developed and shared scripts and modifications to the open source code base.

In this lightning talk session, speakers will share how they are using BitCurator tools as part of their digital curation workflow and how they have expanded BitCurator tools to meet the needs of their institution. The session will also allow time for forum participants to ask questions and share their integration challenges and outcomes.
12:00 – 1:30pm Lunch
1:30 – 2:45pm Breakouts: Where Should Access Happen?
As processes for acquiring, analyzing, and describing electronic records stabilize, institutions invariably consider access to such materials. Where and how will researchers interact with digital archives? What tools should be available to them? What is the Web’s role in access?

In this breakout session, forum participants will divide into groups to discuss the decision points involved in providing access to born-digital archival materials. The session will begin with a quick brainstorm topics before breaking out. Discussion facilitators will have several topics in mind, but participants are encouraged to have their own discussion topics and provocative statements.
2:45 – 3:00 Break
3:00 – 4:00pm Panel: Integration with other systems
Acquisitions and processing workflows often end with a set of output files from various digital curation software tools, including both content and metadata. How does an electronic records program ensure that the output files can integrate with new or existing platforms for long term preservation? In this session, panelists will discuss their experience with different preservation and description systems, including both open source and licensed systems, and how they have approached integrating the output of their workflows into those systems.
4:00 – 4:30pm Wrap up and Future discussion

Accommodations
Please see the list of nearby hotels below.

[The Carolina Inn](http://www.carolinainn.com/) 211 Pittsboro Street
Chapel Hill, NC 27516
Tel 800.962.8519
(This is the closest option. It is on the UNC Campus, just a couple of blocks from Wilson Library.)

[Hampton Inn & Suites Chapel Hill Carrboro/Downtown](http://hamptoninn3.hilton.com/en/hotels/north-carolina/hampton-inn-and-suites-chapel-hill-carrboro-downtown-RDUCOHX/index.html)
370 East Main Street, Unit 100
Carrboro, North Carolina 27510
Tel 919.969.6988
(Walkable distance)

[Holiday Inn Express Chapel Hill](http://www.ihg.com/holidayinnexpress/hotels/us/en/chapel-hill/rdufr/hoteldetail)
6119 Farrington Road
Chapel Hill, NC 27517
Tel 919.489.7555

[Aloft Chapel Hill](http://www.aloftchapelhill.com/)
1001 South Hamilton Road
Chapel Hill, NC 27517
Tel 866.716.8143
(Shuttle buses available)

### Registration now open for BitCurator User Forum 2016! (originally published November 6, 2015)

**BitCurator User Forum 2016**
Join BitCurator users from around the globe as we discuss how we are using the BitCurator software environment. [Hosted by the BitCurator Consortium (BCC)](http://bitcuratorconsortium.org/), this event will be grounded in the practical, real-world experiences of digital archivists and digital curation experts. Come prepared to discuss your current challenges, share emerging BitCurator integrations and workflows, and address the “now what” of handling your digital forensics outputs.

**Date:** 15 January 2016
Place: Pleasants Family Assembly Room, Wilson Library, University of North Carolina, Chapel Hill, North Carolina

**Registration**
General Registration – $30
Student Registration – $15
BitCurator Consortium Member Registration – Free

[Register now!](https://bitcuratorconsortium.org/events/buf2016/registration)

### iPRES2015 is here! Plus BitCurator Social Mixer (originally published October 31, 2015)

Coming to iPRES2015 next week?
The BitCurator Social Mixer will be taking place at the [Back Bar, Top of the Hill](http://www.thetopofthehill.com/back-bar2/#back-bar) next Thursday evening, November 5th from 7pm-9pm.
We will have hors d’oeuvres, BitCurator stickers, and buttons! And lots to chat about.
[Reserve your spot here!](http://t.co/eQ4dd7QSWG)

We also wanted to draw your attention to the [Conference Amplification page](http://ipres2015.web.unc.edu/ipres-amplified/). Networking and engagement are huge parts of any conference and we’ve devised a few special sessions in the conference programme that we really want you to participate in.

See the [iPRES 2015 Full Program](http://ipres2015.web.unc.edu/ipres-2015-program/) and [Program at a Glance](http://ipres2015.web.unc.edu/files/2015/10/ipres2015-program-at-a-glance.pdf) and the [list of posters and demos](http://ipres2015.web.unc.edu/files/2014/12/ipres2015-posters-demos.pdf).

When tweeting about iPRES 2015, we recommend that you use the hashtag #ipres2015.
Both of the [keynotes will be livestreamed](http://ipres2015.web.unc.edu/home/keynote-speakers/).

Hope everyone has a great week!

### Seeking participants for Open-Source Software workshop at iPRES2015 (originally published September 22, 2015)

Workshop: Using Open-Source Tools to Fulfill Digital Preservation Requirements
[International Conference on Digital Preservation (iPRES)](https://ipres2015.web.unc.edu/)
Friday, November 6, 2015
Chapel Hill, NC, USA

The workshop offers a space to talk about open-source software for digital preservation, and the particular challenges of developing systems and integrating them into local environments and workflows.
Topics will include current efforts and grant-funded initiatives to integrate different open source archival software tools; the development of workflows involving multiple open source tools for digital preservation, forensics, discovery and access; and the identification of gaps which may need filled by these or other tools.

Interested parties should submit a short summary (one page maximum) of a demonstration or case study they would like to present. These contributions will serve as the basis for the tool demonstration and case study portions of the day. The workshop organizers will serve as panelists during the third portion of the day and facilitators for break-out group discussions.

Please send your submissions to: oss4pres@unc.edu by Friday, October 9.

You can also send any questions to the address above.

Submission will be reviewed to ensure relevance to the themes of the event. If you would like to be considered for the workshop in time to register for iPRES at the early bird rate (before October 1), please make your submission as soon as possible, and we will do our best to review it quickly.

We hope to see you there.

Organizers
Christine Di Bella
ArchivesSpace

Max Eckard
University of Michigan

Christopher (Cal) Lee
University of North Carolina

Sam Meister
Educopia Institute

Courtney Mumma
Internet Archive

Michael Shallcross
University of Michigan

Bradley Westbrook
ArchivesSpace

### Save the Dates – Announcing CurateGear and BitCurator Users Forum (originally published September 14, 2015)


Curate Gear 2016 – Thursday, January 14th, 2016
2nd Annual BitCurator User Forum – Friday, January 15th, 2016

January will once again be a big month in Chapel Hill for those interested in digital curation. On January 14, we’ll be hosting CurateGear 2016: Enabling the Curation of Digital Collections. This will be the fifth year that we’ve run this interactive day-long event focused on digital curation tools and methods. Participants see demonstrations, hear about the latest developments, and discuss application in professional contexts. We don’t yet have the program for 2016, but you can get a sense of the content and format by visiting the agendas from previous years:

[http://ils.unc.edu/digccurr/curategear2015.html](http://ils.unc.edu/digccurr/curategear2015.html)
[http://ils.unc.edu/digccurr/curategear2014.html](http://ils.unc.edu/digccurr/curategear2014.html)
[http://ils.unc.edu/digccurr/curategear2013.html](http://ils.unc.edu/digccurr/curategear2013.html)
[http://ils.unc.edu/digccurr/2012symposium.html](http://ils.unc.edu/digccurr/2012symposium.html)

On January 15, we’ll be running the second BitCurator Users Forum, hosted by the [BitCurator Consortium](https://bitcuratorconsortium.org/).

You can see information about last year’s BUF at:
[http://educopia.org/events/buf2015](http://educopia.org/events/buf2015)

The BCC Program Committee will be developing the agenda for this year.
Stay tuned for further information.

We hope to see you in Chapel Hill in January!

### Webinar on Using BitCurator (originally published August 15, 2015)

In this webinar given to members of the Association of Southern Research Libraries (ASERL), Matthew Farrell from Duke University Archives describes his work in digital forensics and the use of BitCurator at the Rubenstein Library. In addition to serving as the Digital Records Archivist at Duke, Farrell is also a member of the BitCurator Access Advisory Board.

[Presentation slides](http://www.aserl.org/wp-content/uploads/2015/07/BitCurator_Overview_Farrell_ASERL.pdf)

### BitCurator Takes Vienna! (originally published June 1, 2015)

Cal and Kam just returned from teaching a one-day workshop at the Austrian Institute of Technology (AIT) in Vienna, Austria! The workshop was sponsored by the [Open Preservation Foundation](http://openpreservation.org/), which seeks to promote best practices for the long-term preservation of digital cultural heritage materials.

During the workshop, participants were able to gain hands-on experience using BitCurator tools, including our latest developments with [BitCurator Access](https://github.com/bitcurator/bitcurator-access/wiki). Participants were encouraged to bring disk images from their own collections, in an effort to present and discuss real-world use cases faced by institutions. The workshop focused on using the BitCurator environment to assist with various aspects of digital curation, including pre-imaging data triage; forensic disk imaging; file system analysis and reporting; identification of private and individually identifying information; and export of technical and other metadata. Workshop participants came from five different European countries: Austria, Denmark, Germany, Netherlands, and the United Kingdom.

### BitCurator Access Software Developer Needed! (originally published May 21, 2015)

Would you like to help build software to automatically redact private and sensitive information from large data objects such as disk images?
The [BitCurator Access team](https://github.com/bitcurator/bitcurator-access/wiki) is looking for a software developer to join us during the summer.

The Software Developer will write, test and document software to redact – at both the block level and the file level – patterns identified within born-digital materials. S/he will report to Kam Woods, the Technical Lead of the BitCurator Access project.

**Required:**
– At least one year of Python development experience
– Working knowledge of file system structures and modern file system metadata
– Working knowledge of XML schema design and Python libraries/wrappers to manipulate XML structures (e.g. Expat, ElementTree)
– Must be comfortable using revision control with git and GitHub
– Working knowledge of Linux development environments

**Desirable:**
– Prior experience with open source digital forensics libraries and tools (e.g. The Sleuth Kit, libewf, Digital Forensics XML)
– Familiarity with Python scientific and data analysis libraries (SciPy and Pandas in particular)

**Compensation:**
Up to $25 per hour based on experience. Work to be performed over the summer.

**About BitCurator Access:**
BitCurator Access is an Andrew W. Mellon grant-funded project housed in the School of Library and Information Science at UNC. Our team is working on bringing tools and techniques from the world of digital forensics to libraries, archives, and museums, enabling long-term access to complex legacy digital materials.

If you have any questions about this position, please contact us at bitcurator@gmail.com.

The University of North Carolina at Chapel Hill is an equal opportunity, affirmative action employer and welcomes all to apply regardless of race, color, gender, national origin, age, religion, genetic information, sexual orientation, gender identity or gender expression.
We also encourage protected veterans and individuals with disabilities to apply.

To apply, please go to: [http://unc.peopleadmin.com/postings/75915](http://unc.peopleadmin.com/postings/75915)

### BitCurator Consortium Internship (originally published May 1, 2015)

The BitCurator Consortium (BCC) and The Educopia Institute are looking to hire an intern. To learn more about this opportunity, please read below!

**Description**
Responsible to: Educopia Executive Director

The BitCurator Consortium intern will be responsible for the management of programmatic activities for the BitCurator Consortium (BCC). The intern will be a self-starter with a passionate belief in the importance of digital preservation activities in archives, libraries, and museums.

This position will bear responsibility for a variety of administrative and research-oriented tasks, including: proofreading documents, managing scheduling, taking minutes at meetings, assisting with event hosting, assisting with outreach activities, drafting and updating documentation, and researching best practices for model policies.

The intern will be expected to work 10-15 hours per week, and will be paid $12 per hour.

**Responsibilities include:**
1. Maintaining content on the BCC website and affiliated resources (e.g., training videos and presentations, bibliography)
2. Making arrangements and sending reminders for meetings with members
3. Recording and disseminating detailed meeting minutes
4. Preparing BCC outreach communications and instruments for conferences and other hosted events
5. Assisting with the creation and population of a library of model documents (policies, workflows, contracts, etc)
6. Assisting with the update and revision of training materials and “how to” resources
7. Assisting with the creation of training and professional development activities/proposals

**Qualifications**
– Exceptional written and oral communication skills
– Demonstrated interest and involvement in the digital library and digital preservation communities
– Ability to work under pressure, to adjust to change, to handle multiple tasks, and to coordinate the work of extended groups of member representatives

**Preferred**
– Experience in managing collaborative projects
– Proven ability to produce/execute reports and project plans

**Instructions to applicants**
Please submit a resume, cover letter, and three professional references to Katherine Skinner (Executive Director, Educopia):
katherine@educopia.org. Application deadline is May 29, 2015. Candidates will be considered until the position is filled.

The Educopia Institute is an Equal Opportunity/Affirmative Action Institution committed to diversity in its employment and educational programs, thereby creating a welcoming environment for everyone.

### Save the Date! Announcing the 2nd Annual BitCurator Social Mixer at SAA (originally published April 29, 2015)

We are excited to announce that the 2nd Annual BitCurator Social Mixer will be held at the 2015 [Society of American Archivists (SAA) Annual Meeting](http://www2.archivists.org/am2015#.VUEqDCFVhBc). The mixer will take place at [Porcelli’s Bistro](http://porcellibistro.com/) on Wednesday, August 19th at 730pm. Hors d’oeuvres will be provided. Please join us for an opportunity to learn how other colleagues are using BitCurator and to talk through strategies and implementation options.

We’d like to get a headcount of possible interested parties, so please RSVP below.

### Registration now open for OPF Digital Forensics Workshop in Vienna! (originally published April 21, 2015)

Registration is now open for our next event “From the Toolbox: BitCurator Digital Forensics workshop” which takes place on May 29, 2015 at the AIT Austrian Institute of Technology in Vienna.

**Overview**

This one-day OPF workshop offers the opportunity to learn how digital forensics and the use of disk images can support your digital preservation workflows. Supported by expert facilitators Cal Lee and Kam Woods from the University of North Carolina, participants will get hands-on experience using the BitCurator tools including the latest developments with BitCurator Access. The BitCurator Environment is a suite of open source digital forensics and data analysis tools to help collecting institutions (libraries, archives, and museums) process and provide access to born-digital materials.

**Who should attend?**

This workshop is intended for archivists, manuscript curators, librarians or others who are responsible for acquiring, transferring and/or providing access collections of born-digital materials, particularly those that are received on removable media. We will assume that participants are familiar with basic digital curation issues and practices.

Though it is not mandatory, participants will ideally know how to create disk images; generate and verify cryptographic hashes of files; and examine the contents of a file in a hex editor. It will also be helpful to understand the role and purpose of filesystems, file headers, and file signatures. Knowledge of Linux command line operations will also be beneficial, but is not a necessary prerequisite to participation. We’ll be on hand to help with tasks, and many of the tools have graphic user interfaces.

**Why attend?**

Participants will learn about and get experience using BitCurator environment tools that can assist with various aspects of digital curation, including pre-imaging data triage; forensic disk imaging; file system analysis and reporting; identification of private and individually identifying information; and export of technical and other metadata. They will also learn about tools that are currently available but undergoing significant further development for providing access to data from disk images and redacting sensitive content. Participants should leave with a practical understanding of how to apply these tools in their own institutions and with contacts in peer institutions who are undertaking similar work.

[More information, including registration and agenda.](http://wiki.opf-labs.org/display/KB/2015-05-29+From+the+Toolbox+-+BitCurator+Digital+Forensics+workshop)

OPF members are invited to attend free of charge. The price for non-members is 75 Euros.

### Guest Post: Walker Sampson on Disk Imaging Workflow (originally published February 4, 2015)

Below is a guest post by [Walker Sampson](https://wsampson.wordpress.com/), the Digital Archivist at the University of Colorado Boulder. Walker describes the disk imaging workflow he presented at the first ever BitCurator User Forum held January 9th, 2015.

![Media capture](https://bitcurator.github.io/images/posts/Capture.png)

It was a real pleasure discussing workflows with fellow practitioners at the BitCurator Users Forum this year. Many thanks to Matt Farrell at Duke and Kari Smith at MIT for presenting with me, and to Farrell again for putting together and directing our panel.

I have pictured above a synopsis of my disk imaging workflow, which relies strongly on student help. Students take floppy disks from initial photography to imaging, mount testing, documentation of the results, and rehousing.

The disk is photographed to record the labeling information, which can be quite extensive (one collection of media art contains many disks with a printout of the disk’s file listing, along with the official label of the artists’ studio). A photograph also provides a visual reference for the future should we try to relocate the original media.

Students are trained to connect the KryoFlux floppy disk controller and a vintage disk drive to the host machine, which runs a copy of BitCurator. They are also trained on the KryoFlux GUI, and use this software for most of the disk imaging. While we have the FC5025 controller and software, KryoFlux is the device of choice given its greater versatility and ability to record flux timings for each track of the floppy disk. Within the KryoFlux GUI, students set the encoding formats to MFM (modified frequency modulation, a common coding for many IBM PC formatted disks) and the preservation stream by default, as this produces an accurate image for most disks. In the case that it does not, students are trained to run other disk encodings against the preservation stream files to attempt a positive disk image that can be mounted. In most cases, the disk turns out to be in a less common Apple or Commodore format.

The resulting log file, preservation tracks, image file, and disk photograph are saved in a folder. The student then runs a mount test through BitCurator’s mounting script. The results of the student’s disk imaging run are recorded in a row in a collection spreadsheet, which denotes the disk image name, date, their name, the disk drive used (we have different drives in use), the disk imaging device used, any bad sectors found, whether the disk mounts, and if there is a photograph accompanying the disk. The student than rehouses the disk in a Hollinger box. Disk collections which contain office documents and correspondence are candidates for floppy disk deaccessioning; collections for which the floppies are integral to the content and process of the donator, such as the media art collection mentioned above, are not.  

I check the students’ work at the end of the week. If disks have bad sectors or do not mount I investigate those disk images and attempt new reads if necessary. Besides the local backup, I run BagIt on the cumulative work of the student every week and upload that bag to our servers, which run their own backup routine. When the collection is complete, I do the same for the entire collection and remove the in-progress bags.

This workflow emphasizes the capture of disk images foremost. Analysis and description of the disk content is provided intermittently by myself, and batch runs of bulk_extractor and fiwalk on the disk images will be performed at a later time. Import into a formal digital archive software will occur down the road as well – a work in progress for us presently. I hope this workflow can help others who may not have a repository in place, but nevertheless need to rescue content from legacy media in a manner that will allow more refined processing in the future.

### BUF 2015 Wrap Up! (originally published January 20, 2015)

The First Annual BitCurator User Forum took place last Friday, January 9th at the Pleasants Family Assembly Room in Wilson Library on the campus of the University of North Carolina Chapel Hill. The Forum was attended by approximately forty practitioners from around the world, focused around three panel discussions. The goal of the forum was to describe best practices, discuss challenges in implementing the environment, share strategies for integrating BitCurator into institutional workflows, and to provide opportunities for collaborations on future work.

![User forum members on steps](https://bitcurator.github.io/images/posts/IMG_5382.jpg)

The first panel was chaired by Erika Farr, head of Digital Archives at the Manuscripts, Archives, and Rare Book Library at Emory University. She was joined by Euan Cochrane, Digital Preservation Manager at the Yale University Library and Brian Dietz, the Digital Program Librarian for Special Collections at the North Carolina State University Libraries. The session focused on options for disk image formats (particularly the Encase image format, the Advanced Forensic Format, and raw) and the criteria different institutions use to choose a format for a particular type of media. The panelists and the audience discussed the pros and cons of different formats and will begin to articulate general criteria for format selection.

![Panel discussion](https://bitcurator.github.io/images/posts/B66zhjXCAAAOkT8.jpg)

Matthew Farrell, Digital Records Archivist at Duke University, chaired the next panel on workflow exchanges. He was joined by Walker Sampson, Digital Archivist at the University of Colorado Boulder, and Kari Smith, Digital Archivist at the Massachusetts Institute of Technology Libraries. This panel focused on the use of BitCurator tools and output in each institutions’ archival workflows. Each panelist gave a quick overview of their workflow and then addressed specifically how they integrated BitCurator into their existing preservation systems, collection management systems and descriptive workflows, and their appraisal workflows. Look for an upcoming post from Walker Sampson next week describing his approach at UC Boulder.

![Appraisal workflows discussion](https://bitcurator.github.io/images/posts/IMG_53861.jpg)

Christopher (Cal) Lee, the Frances Carroll McColl Term Professor in the School of Information and Library Science at the University of North Carolina Chapel Hill and the Principle Investigator of the BitCurator Access project, chaired the final panel on future work integrating BitCurator with other tools and environments. The other panelists were Kam Woods, Research Scientist at UNC SILS and co-Principle Investigator on the BitCurator Access project; Don Mennerich, Digital Archivist at New York University; Zach Vowell, Digital Archivist at Cal Poly, and Brad Westbrook, Program Manager at ArchivesSpace. Each panelist gave a brief presentation about current development activities they were working on. Following that, the panel held a larger group discussion with the forum about the biggest integration challenges and specific opportunities at their institutions.

![Challenges discussion](https://bitcurator.github.io/images/posts/4.jpg)

The BitCurator User Forum provided a space for this emerging community to highlight issues and concerns, and to share strategies and best practices. We are very grateful to the [Educopia Institute](http://www.educopia.org/) for hosting the forum, and the Andrew W. Mellon Foundation for providing funding for the event.

In the coming weeks, some of our discussion panelists will be providing guest posts about their individual presentations to the forum. Stay tuned!

## 2014 Posts

### BitCurator User Forum – Register now! (originally published December 23, 2014)

REMINDER:
The 1st Annual [BitCurator User Forum](http://educopia.org/events/BUF2015) will be held on Friday, January 9th at UNC Chapel Hill.
[Registration](http://educopia.org/events/buf2015/registration) is still open!

Join BitCurator users from around the globe for a hands-on day focused on current use and future development of the BitCurator digital software environment. Hosted by the BitCurator Consortium (BCC), this event will be grounded in the practical, boots-on-the-ground experiences of digital archivists and curators. Come wrestle with current challenges—engage in disc image format debates, investigate emerging BitCurator integrations and workflows, and discuss the “now what” of handling your digital forensics outputs.

General Registration – $30
Student Registration – $15
BitCurator Consortium Member Registration – Free

Take a sneak peak at the [scheduled program](http://educopia.org/sites/educopia.org/files/BitCurator_Users_Forum_2015_Program_0.pdf).

### New white paper: “From Code to Community: Building and Sustaining BitCurator through Community Engagement” (originally published November 5, 2014)

The BitCurator team is pleased to announce the availability of [From Code to Community: Building and Sustaining BitCurator through Community Engagement](https://kamwoods.net/publications/code-to-community.pdf). This white paper summarizes the activities undertaken during the second phase of the BitCurator project, which ran from October 1, 2013 to September 29, 2014. It describes efforts taken to develop and support an open-source software project through the cultivation of the BitCurator user community.

### New case study in latest issue of IJDC! (originally published October 31, 2014)

The latest issue of [International Journal of Digital Curation](http://ijdc.net/) (IJDC) features a paper written by [Sam Meister, Digital Archivist at the University of Montana](http://www.linkedin.com/pub/sam-meister/a/998/639) and [Alexandra Chassanoff, BitCurator Project Manager and doctoral student at UNC-Chapel Hill](http://achass.web.unc.edu/). Using a case study approach, the article explores how BitCurator can support digital curation activities in archival workflows.

[Integrating Digital Forensics Techniques into Curatorial Tasks: A Case Study](http://www.ijdc.net/index.php/ijdc/article/view/9.2.6/364)

### Announcement: BitCurator Access! (originally published October 21, 2014)

Press Release ([pdf](http://www.bitcurator.net/wp-content/uploads/2014/10/BCAccess-PressRelease.pdf))
Release date:
October 21, 2014
**Andrew W. Mellon Foundation Grant Supports Improving Access to Born-Digital Collections for Collecting Institutions**

CHAPEL HILL – [The University of North Carolina at Chapel Hill’s School of Information and Library Science (SILS)](http://sils.unc.edu/) has received a grant for $750,000 from the [Andrew W. Mellon Foundation](https://mellon.org) for a project that focuses on simplifying and improving access to the contents of disk images in born-digital collections for use by libraries, archives, and museums (LAMs).

[The BitCurator Access project](https://bitcurator.github.io/bitcurator-access-project/) will develop open-source software that supports the provision of access to disk images through three exploratory approaches: (1) building tools to support web-based services, (2) enabling the export of file systems and associated metadata, (3) and the use of emulation environments. Also closely associated with these access goals is redaction. BitCurator Access will develop tools to redact files, file system metadata, and targeted bitstreams within disks or directories.

BitCurator Access builds on previous work of the [BitCurator project](https://bitcurator.github.io/bitcurator-project), a three year, collaborative effort between SILS and the [Maryland Institute for Technology in the Humanities (MITH)](http://mith.umd.edu/) at the University of Maryland. The project developed, packaged, and documented open source digital forensics tools to allow LAMS to advance many core digital curation goals, including: creation of authentic copies of data on disks; reflection of the original order of materials; establishment of more trustworthy chains of custody; discovery and exposure of associated contextual information; and identification of sensitive information that should be filtered, redacted or masked in appropriate ways.

“Many LAMs within the US and internationally are using these tools and methods to generate disk images, extract metadata to support ongoing preservation tasks, and store the resulting data in dedicated servers or shared network spaces,” said Dr. Christopher (Cal) Lee, principal investigator of the BitCurator Access project. “However, there is currently very limited support for provision of access to the contents of the disk images or associated metadata.”

Kam Woods, Research Scientist at SILS, will be the Co-Principle Investigator and Technical Lead for the BitCurator Access project. Sunitha Misra, a recent graduate of SILS’ MSIS program, will serve as software developer. Alexandra Chassanoff, a SILS doctoral candidate, will serve as the Project Manager. An advisory group of external partners with significant relevant experience will provide guidance and expertise.

For more information about the project, please visit the main BitCurator web site at: [https://bitcurator.github.io/](https://bitcurator.github.io) and follow @bitcurator on Twitter.

### Using BitCurator to investigate literary archives (originally published October 8, 2014)

Curious about how scholars might use BitCurator to investigate and analyze born-digital materials in literary archives?  [In this post](http://britishlibrary.typepad.co.uk/digital-scholarship/2014/09/first-digital-lives-research-workshop-2014-at-the-british-library.html), Jeremy Leighton John, curator at the British Library, describes using the BitCurator environment to dig deeper into the born-digital archives of author [Hanif Kureishi](http://en.wikipedia.org/wiki/Hanif_Kureishi).

We’ll continue to profile real-world use cases on in upcoming blog posts – if you’d like to contribute a guest post on how you have used BitCurator, please contact us!

### BitCurator 1.0 Release! (originally published September 25, 2014)

The BitCurator team is pleased to announce the 1.0 release of the BitCurator environment, now available for [download on our release portal](https://github.com/BitCurator/bitcurator-distro/wiki/Releases) or by following the direct links below:

[The BitCurator 1.0.0 Virtual Machine](https://github.com/BitCurator/bitcurator-distro/wiki/Releases) – 2.6GB
[The BitCurator 1.0.0 Installation ISO](https://github.com/BitCurator/bitcurator-distro/wiki/Releases) – 2.3GB

BitCurator 1.0 is the culmination of three years of work by our team to provide professionals working in collecting institutions with an integrated environment of open source digital forensics tools geared towards their specific needs. The BitCurator team has approached this challenge by developing new software to assist with born-digital media processing, and by curating a collection of mature, reliable third-party software projects and libraries into a single, well documented system.

As with previous releases, 1.0 is distributed as a VirtualBox virtual machine disk image and as a bootable (“Live”) ISO image. The BitCurator virtual machine can be run on any 64-bit operating system capable of running VirtualBox, including Windows 7, Windows 8, Mac OS X 10.7+, and most modern Linux distributions. If you would prefer to create your own virtual machine, the BitCurator ISO image can be used as an installation source. The BitCurator ISO may also be used to install BitCurator on a dedicated host.

BitCurator is unique among the digital forensics oriented Linux distributions available today, not only because of the focus on the needs of libraries, archives, and museums, but because of the care that has been taken to ensure the functionality, relevance, and completeness of each tool within the environment. Updated information on these tools can always be found in the [Tools in the BitCurator Environment](https://confluence.educopia.org/display/BC/Tools) section of the BitCurator Environment wiki.

Of particular note: the 1.0 release introduces an improved version of the BitCurator Disk Image Access tool, a GUI interface allowing you to browse the contents (both regular and deleted/unallocated files) of raw and forensically packaged disk images. The updated tool includes stability and performance enhancements when working with FAT, NTFS, and HFS+ volumes, including better handling of multi-volume disk images and real-time feedback on file export actions.

Our Quickstart guide to help you get started working with the environment can be found on the wiki, in the Documentation folder on the BitCurator environment desktop, or by following [this direct link](https://github.com/BitCurator/bitcurator-distro/wiki/Releases#quickstart-guide). As with previous releases, the BitCurator environment is built using a customized version of Ubuntu 14.04 (64-bit). For best performance, we recommend a host machine with an Intel Core i5 (or equivalent) and at least 8GB of RAM.

Many of you have been following our progress on the user forum for a couple of years now. In just the past 12 months, we have had 30 official releases, introduced three new GUI-based tools, and conducted dozens of training workshops both in the US and internationally. We’re committed to ensuring the ongoing development of BitCurator to meet the needs of the community. To this end, we’ve created the BitCurator Consortium (BCC), an independent, community-led membership association that will serve as the administrative, development, and community support center for the BitCurator environment.

Details on how to join can be found on our [BitCurator Consortium Membership](http://www.bitcurator.net/bcc-membership/) page. Institutional membership costs are modest; membership confers voting rights, prioritizes enhancement requests, and offers discounts to future BCC events. Charter memberships are available through December 2014, and general membership enrollment is open.

### BitCurator Consortium Launches! (originally published September 15, 2014)

The Educopia Institute is pleased to announce the launch of the [BitCurator Consortium (BCC)](http://www.bitcurator.net/bitcurator-consortium/), a new independent, community-led membership association to support the curation of born-digital materials by libraries, archives, and museums. Members of the BitCurator user community have founded BCC to enhance, promote, and explore this growing area of professional activity.

“Managing born-digital acquisitions is becoming a top concern in research libraries, archives, and museums worldwide,” shares co-founder Dr. Christopher (Cal) Lee. “The BCC now provides a crucial hub where curators can learn from each other, share challenges and successes, and together define and advance technical and administrative workflows for born-digital content.” Co-founder Dr. Matthew Kirschenbaum adds: “Tools without actively invested communities wither on the vine, become dead bits. The BCC is not just an extension of BitCurator, in a very real sense it will now become BitCurator.”

Institutions responsible for the curation of born-digital materials are invited to become [members of the BCC](https://bitcuratorconsortium.org/get-involved/). New members will join an active, growing community of practice and gain entry into an international conversation around this emerging set of practices.

Other member benefits include:
• Voting rights
• Eligibility to serve on the BCC Executive Council and Committees
• Professional development and training opportunities
• Subscription to a dedicated BCC member mailing list
• Special registration rates for BCC events

The BCC operates as an affiliated community of the [Educopia Institute](http://educopia.org/), a non-profit organization that advances cultural, scientific, and scholarly institutions by catalyzing networks and collaborative communities to facilitate collective impact.

Learn more about BCC and its growing network of libraries, archives, and museums [here](https://bitcuratorconsortium.org/)!
Read/download the official press release [here](http://www.bitcurator.net/wp-content/uploads/2014/09/Press-Release-BCC.pdf)!

### BitCurator Users Gathering @ Archives\*Records – August 12, 2014 (originally published July 23, 2014)

Please join us for a gathering of BitCurator users on the evening of August 12th after the SAA Research Forum from 5:30PM to 7:30PM. Come meet other BitCurator users and share your experiences working with digital forensics and BitCurator. In addition to collaborating with other BitCurator users, meet with BitCurator Co-PI’s Cal Lee and Matt Kirschenbaum, and BitCurator Community Lead Porter Olsen. We will discuss the project thus far, recent developments, and BitCurator going forward. Appetizers will be provided, so please come and join us! Email Porter at polsen (at) umd dot edu if you have any questions.

**Who:** BitCurator users and prospective users

**When:** The evening of August 12, 2014 from 5:30PM to 7:30PM

**Where:** The second floor of the [Black Squirrel](http://www.blacksquirreldc.com/) gastropub located at 2427 18th Street NW
Washington, D.C. 20009, a fifteen minute walk from the Washington Marriott Wardman Park hotel where the SAA Annual Conference is being held.

To join us, please fill out the brief form below. We will email attendees with gathering details as we get closer to the event date.

### BitCurator Consortium — Membership Now Open (originally published July 8, 2014)

The BitCurator Consortium (BCC) is an independent, community-led membership association that will serve as the host and center of administrative, user and community support for the BitCurator environment.  Its purpose is to support curation of born-digital materials through the application of open-source digital forensics tools by institutions responsible for such materials.

The BitCurator project (2011-2014), funded by the Andrew W. Mellon Foundation, has developed, packaged and documented open-source digital forensics tools to allow libraries, archives and museums (LAMs) to extract digital materials from removable media in ways that reflect the metadata and ensure the integrity of the materials, allowing users to make sense of materials and understand their context, and preventing inadvertent disclosure of sensitive data.  The BitCurator project has also engaged with interested professionals, through conferences, specialized events, online interactions, and site visits.  Together, these tools and relationships provide a strong foundation upon which the BitCurator Consortium now builds.

**The Software**

The BitCurator software is freely distributed under an open source license.  It can be installed as a Linux environment; run as a virtual machine on top of most contemporary operating systems; or run as individual software tools, packages, support scripts, and documentation.

Tools in the BitCurator environment – both those produced by the project team and those from third-party developers – can advance core curation activities, including (but not limited to):

* Reduce the risk of inadvertent changes to content through software-based write-blocking
* Create authentic copies of content through disk imaging and cryptographic hashing
* Mount forensically packaged disk images to view and export their content
* Reflect original order of materials through capture of filesystem metadata
* Establish trustworthy chains of custody through documentation of curatorial actions (log files, PREMIS records)
* Generate reports that characterize the contents of disks and directories
* Identify and document duplicate files
* Discover and expose associated contextual information
* Identify sensitive information that should be filtered, redacted or masked in appropriate ways
* Export contents of disks and directories for inclusion in Archival Information Packages and Dissemination Information Packages

**Consortium Membership**

Institutions responsible for the curation of born-digital materials – especially those held or acquired on digital storage media – are invited to participate in the BitCurator Consortium. Membership is open to institutions in all sectors and all nations.  The BCC envisions a robust network of institutions committed to enhancing, promoting, and exploring this growing area of activity.

There are two categories of BCC membership: Charter and General. Charter Members will play an early, active role in the shaping of the BitCurator Consortium’s governance, ongoing development, and overall sustainability.  Charter Membership is a one-time membership option, available only through December 31, 2014.

The most important member benefit is assurance that the BitCurator software will persist and evolve in future years. Other membership benefits include:

*General Members:*

* Access to a BCC help desk
* Prioritization in future enhancement requests
* Dedicated educational offerings
* Voting rights
* Eligibility to serve on the BCC Executive Council and Committees
* Service opportunities
* Community engagement and networking
* Professional development and training
* Subscription to a dedicated BCC member mailing list
* Special rates for BCC events, including the annual BitCurator User Forum

*Charter Members – all General Member benefits and:*

* Opportunity to participate in and shape the initial BitCurator Consortium Executive Council and BitCurator Consortium Committees, including exclusive eligibility for election or appointment to the Executive Council during the charter period
* Participation in the development of the initial BitCurator Consortium user, technical and service roadmaps.
* Recognition through the placement of your institution name, logo and link on the BitCurator Consortium web site.
* Use of the “BitCurator Consortium Charter Member” icon
* During the Charter period (June-December 2014), members can take advantage of the following rates (subject to potential changes in the future):

Dues for Charter Members in the first year are $5000 (US).  After the first year of membership, dues will be the same as those of General Members.

General Member dues are $2000 (US) per institution per year, for a three-year period with annual billing opportunities.  Members can pay in full for their three-year period during their first six months of membership to lock in the above rates.

– If you’re interested in joining the BitCurator Consortium, contact Cal Lee – callee {at} ils [dot] unc {dot} edu

– For information about the BitCurator Consortium, visit: [https://bitcuratorconsortium.org/](https://bitcuratorconsortium.org)

– For information about the BitCurator software and user community, visit: [https://bitcurator.github.io](https://bitcurator.github.io)

The BCC is administered by the Educopia Institute, a non-profit that advances cultural, scientific, and scholarly institutions by catalyzing networks and collaborative communities.

### Alternatives for Imaging a Mac Laptop (originally posted May 7, 2014)

*Original post by Amanda Visconti. Minor updates in July 2018 to resolve outdated links and media.*

Last week, I wrote about how to forensically image the internal hard drive on a Mac laptop without needing to physically remove the drive. If your workspace doesn’t have the necessary tools to follow that tutorial (a firewire cable, a firewire port on the Mac you’re imaging, and a firewire port on a PC partitioned with BitCurator), we offer an alternative in this post.

The Mac laptop we wanted to forensically image.
The Mac laptop we wanted to forensically image.
Other Options for Imaging Mac Laptops

We recognize that you might not have the correct devices on hand to follow the instructions in the previous post. In that case, you may want to open the laptop to temporarily remove the hard drive for forensic imaging within the BitCurator environment, which means you’ll need a cable that connects a hard drive to your imaging computer (probably a SATA cable). You can also opt to make a forensics image outside BitCurator and then import the image into BitCurator for exploration.

Note that the issue complicating this imaging process is specific to Mac laptops; Linux and Windows laptops wouldn’t require target disk mode and the trouble that causes. Target disk mode works with other Macs (perhaps obviously) and Linux machines; I wasn’t able to get a Windows machine to recognize the Mac laptop in target disk mode. I’ve read that commercial software called MacDrive (currently about $50 for use on one PC) will let you connect the a Mac in target disk mode to a PC, but this would not make the Mac drive also available in the Windows computer’s BitCurator VM; unfortunately, VirtualBox is unable to take firewire input. It’s possible you could get around this issue by using other virtualization software, but VirtualBox is the best free/open-source option.

That leaves us with using either a Mac or Linux machine to create our backup of the Mac laptop; in our example, I used a Mac to create the backups. We’ll walk you through how to first lessen the risk of tampering with a laptop’s insides by securing a forensic image outside of BitCurator.

Why Backup?

Opening up the laptop, removing the drive, and later trying to put everything back risks the laptop refusing to start or otherwise being damaged: maybe you break something, or can’t get things to fit back together. If you don’t have another way to gather a forensics disk image packaged with metadata about the imaging, though, opening the laptop up can be an acceptable risk. All computers fail eventually, and we’d rather have a good forensics disk image of the laptop now, than more years with the laptop working but no forensics image preserved. We thus recommend you forensically image the laptop’s hard drive before opening it, or choose to create a forensics image with one of the non-BitCurator options discussed below and import the image into BitCurator. Opening up the computer is only necessary if none of these forensics imaging programs are right for you, your Mac laptop doesn’t have a firewire port, or if you prefer to do all your forensic work inside the BitCurator environment. For either method, you’ll need a firewire and another Mac (with a firewire port) on which to image the laptop.

Write Blocking

First, we need to protect the laptop from having the connected machine write back to it during the imaging process. This wasn’t a major concern in our example as Larsen’s laptop has already been explored by researchers at MITH—but it’s good practice nonetheless, especially if you use a command-line imaging method, where a simple is-typing could accidentally erase your device. Our WiebeTech Forensic ComboDock works well for most write-blocking purposes, but it doesn’t have the firewire input and output needed to work with a Mac in target disk mode. Tableau T9 Firewire Forensic Bridge is a hardware option that does accept both firewire input and output, but we didn’t have one on hand. We thus used software write-blocking instead, installing Aaron Burghardt’s Disk Arbitrator to protect the laptop.

Imaging time! Leaving the computers alone during imaging.
Imaging time! Leaving the computers alone during imaging.
A Forensic Disk Image

Begin by putting the Mac laptop you want to image into target disk mode:

The laptop to be imaged (e.g. our Larsen laptop) should be turned off.
Hold down the t key and turn the laptop to be imaged on.
Continue to hold down the t key until the target disk mode image appears on the screen (see photo below).
Mac in target disk mode.
Mac in target disk mode.
You can now connect your firewire cable to both the laptop to be imaged and the Mac (or Linux computer) doing the imaging.

Mac in target mode connected to imaging workstation.
Mac in target mode connected to imaging workstation.
To create a forensics disk image, there are a variety of free and commercial programs that provide graphical interfaces for Mac and Linux, including MacOSXForensics Imager (Mac) and Guymager (Linux; note that Guymager is the imaging software BitCurator incorporates). Commercial options such as FTK Imager also exist. Almost any program that creates the image in an Encase (E01) or AFF forensic disk image format works, as these formats take a raw disk image and wrap metadata about the imaging around it. We haven’t formally evaluated the effectiveness of any programs outside the BitCurator suite, though, so you’ll want to check potential Mac forensic imaging software out yourself and explore the images they create within the BitCurator environment to make certain they captured your device correctly.

Alternatively, you can choose one of the following command line methods—but it’s of utmost importance that you use a write-blocker with these, as mis-typing could erase your device:

If you’re very knowledgeable about using the command line, you may already know how to use dd or dcfldd.
The ForensicsWiki has a detailed tutorial on “Acquiring a Mac OS System with Target Disk Mode” that uses dd and other commands to create a .dmg image, plus instructions on converting the .dmg to an Encase format.
“Macintosh Forensics: A Guide for the Forensically Sound Examination of a Macintosh Computer” by Ryan Kubasiak offers alternative instructions for using dd (use the hyperlinked table of contents to jump to the “Imaging a Target Macintosh” section starting on page 25).
Opening the Laptop to Remove the Hard Drive

After following these steps to make a forensic image of your laptop, you can either opt to import the forensic image into BitCurator and explore the image there, or choose to temporarily remove the hard drive in order to image it directly through BitCurator. If you choose the latter path, you’ll need to search for instructions like these that show how to open your particular model of Mac. If possible, use a guide with many photos to show you how to carefully open, remove, and replace the Mac laptop’s hard drive. I’ve found that sites dedicated to DIY fixing and making, such as iFixit and Instructables, offer good community-moderated tutorials on opening up computers.

In a future post, I’ll discuss what I found while exploring the Larsen laptop disk image using BitCurator. Send us your suggestions for other difficult-to-image use cases, and we’ll cover them in future posts!

Amanda Visconti is a MITH graduate research assistant on the BitCurator project, where she creates user-friendly technical documentation, develops and designs for the web, and researches software usability. As a Literature Ph.D. candidate, she blogs about her digital humanities work regularly at LiteratureGeek.com.

### Forensically Imaging a Mac Laptop for BitCurator Exploration (originally published April 30, 2014)

*Original post by Amanda Visconti. Minor updates in July 2018 to resolve outdated links and media.*

Let’s say a digital beauty like this makes its way into your collection:

The lid of the Larsen laptop is covered in flower and lace doily decals.
The lid of the Larsen laptop is covered in flower and lace doily decals.
BitCurator can aid us in such investigations by freeing Larsen’s laptop data from its storage media (which will fail eventually), capturing important contextual details about Larsen’s original work environment, and helping to ensure the authenticity and integrity of files during forensic processing (see this page on how BitCurator fits into existing archival workflows, or this page on how the individual tools making up the BitCurator suite address particular archival concerns, for more information on what BitCurator can do).

To use BitCurator, we’ll need to figure out how to connect the laptop’s hard drive to the BitCurator environment; this post will explore how you can similarly image your Mac laptop for digital forensic work.

Why is it difficult to image an internal Mac laptop drive?

You can get to work quickly with BitCurator if you’ve got a digital device ready to be connected to your computer: an external hard drive or removed internal hard drive, a floppy disk port, a USB stick, or other devices and the cables to attach them to your host machine.

With a Mac laptop, however, the device isn’t as easy to get at. If it’s a working, explorable laptop, as with Larsen’s, there’s a risk to that working status associated with temporarily physically removing the drive for imaging via a SATA cable—so we’d like to avoid opening the laptop up if possible, and find some other way of imaging the drive.

Mac in target disk mode.
Mac in target disk mode.
Imaging the laptop hard drive by connecting one of its exterior ports (e.g. USB) seems like the way to go, but Macs are finicky about showing up as drives on other computers.

If you want to see your Mac laptop as a drive mounted on another computer (and thus be able to image it), you’ll need to set the laptop to something called Target Disk Mode:

Target Disk Mode Steps

The laptop to be imaged (e.g. our Larsen laptop) should be turned off.
Hold down the t key and turn the laptop to be imaged on.
Continue to hold down the t key until the target disk mode image appears on the screen (see photo example).
You can now attach the target disk via firewire cable to a machine with BitCurator running in a partition, and the Mac laptop should show up as a connected drive like any other connected device.
Unfortunately, target disk mode can only transfer data over a firewire; using other ports/cables such as USB will not work. This presents three problems:

Both your laptop and the machine running BitCurator must have firewire ports to allow for the firewire
You’ll need to be running BitCurator on a partition and not as a virtual machine, as VirtualBox can’t handle firewire input
If you want to use a hardware write-blocker, it will need to have both firewire input and output
This use case is Mac plus laptop-specific: that is, desktop Macs don’t use the compact unibody design of the laptop, so it’s far easier to open the case and connect the hard drive to a machine running BitCurator (thus there is no need to adopt Target Disk Mode). And non-Mac laptops will show up as image-able drives on other machines automatically, without the special needs of the Mac Target Disk Mode.

Our Choice: Imaging with BitCurator on a Partition

Imaging the Larsen Mac laptop using a firewire and PC partitioned with the BitCurator Ubuntu.
Imaging the Larsen Mac laptop using a firewire and PC partitioned with the BitCurator Ubuntu.
Why? We had the necessary components to let BitCurator recognize the Mac laptop as a drive: a firewire cable, a firewire port on the Larsen Mac, and a firewire port on a PC partitioned with BitCurator.

Our hardware write-blocker (WiebeTech Forensic ComboDock), used to protect devices from being written to while we're imaging them.
Our hardware write-blocker (WiebeTech Forensic ComboDock), used to protect devices from being written to while we’re imaging them.
We weren’t able to use our usual hardware write-blocker, as it only takes firewire input but doesn’t output it; BitCurator incorporates a feature that can mount devices safely, however, so we were still able to protect the device from being written back to. Follow these instructions to safely mount devices in BitCurator.

The software write-blocker safely mounts the laptop as a drive.
The software write-blocker safely mounts the laptop as a drive.
Next, we used BitCurator’s bundled Guymager software to forensically image the laptop (see these instructions or this video for steps to use Guymager yourself.) This produced a forensic image of the laptop, which we’ll be further exploring with BitCurator in a future post.

Using BitCurator's Guymager instance to forensically image the laptop.
Using BitCurator’s Guymager instance to forensically image the laptop.
In another future post, I’ll discuss an alternative approach for those of you who couldn’t follow these instructions (e.g. no firewire port, no BitCurator running on a partition).

Send us your suggestions for other difficult-to-image use cases and we’ll cover them in future posts!

Amanda Visconti is a MITH graduate research assistant on the BitCurator project, where she creates user-friendly technical documentation, develops and designs for the web, and researches software usability. As a Literature Ph.D. candidate, she blogs about her digital humanities work regularly at LiteratureGeek.com.

### BitCurator Version 0.8.4 Now Available (originally published April 21, 2014)

Hello everyone,
The latest release of the BitCurator environment (0.8.4) is now available on our release portal. Direct links and MD5 checksums can be found on the wiki, or you can follow the links below:

The BitCurator Virtual Machine – 2.5GB
The BitCurator Installation ISO – 2.2GB

This release includes a range of stability updates and bug fixes. Items of note:

– Floppy disk drive access restored. This had become disabled in the previous release due to a system update to the Ubuntu core.
– Installation bug preventing complete installation on laptops with certain types of webcams fixed.
– File system output in Excel format now includes file format identification field.
– BitCurator configuration file (in /etc/bitcurator/bc_report_config.txt) and supporting software module updated to simplify tuning of report file output. Additional documentation to follow on the wiki.

– VirtualBox additions updated to 4.3.10. Our updated Quickstart guide can be found on the release portal, or in the Documentation folder on the BitCurator environment desktop.

As with previous releases, this environment is built on a 64-bit version of Ubuntu and may be unstable on certain 32-bit host operating systems, or host hardware with less than 4GB of RAM. Please don’t hesitate to post here if you have questions!

### BitCurator Webinar Series: Announcing a Second Session on Digital Forensics Metadata (originally published April 2, 2014)


Due to the interest in this topic, we have added a second session of this webinar to be held on Thursday, April 17th at 11:00am Eastern Time.

Join us for BitCurator’s monthly webinar series on applying digital forensics tools and methods to the preservation of born-digital materials in collecting institutions. The webinar will be held on Thursday, April 17th at 11:00am Eastern Time. You can register for the webinar at https://bitcurator-metadata-s2.eventbrite.com.

This month’s webinar will focus on BitCurator and metadata output, including the following topics:

Metadata produced by the image capture process
File system metadata
An overview of DFXML and export capabilities
PREMIS event system metadata
How BitCurator-generated metadata fits into your archival workflow
There are no prerequisites for this webinar; however, it is designed for users already familiar with the basic operations of the BitCurator environment. The webinar will be roughly one hour with 10 minutes for Q&A at the end.

### BitCurator Webinar on Working with External Media Recording Now Available (originally published March 19, 2014)

For those who were unable to attend February’s webinar on external media and the BitCurator environment, a recording of the event can be viewed here. BitCurator webinar on external media.

### BitCurator Webinar Series: BitCurator and Digital Forensics Metadata Output (originally published March 13, 2014)

Note: Due to a scheduling conflict with one of the presenters, this webinar has been rescheduled for April 9th.

Join us for BitCurator’s montly webinar series on applying digital forensics tools and methods to the preservation of born-digital materials in collecting institutions. The webinar will be held on Wednesday, April 9th at 11:00am EST. You can register for the webinar at https://bitcuratorandmetadata.eventbrite.com.

This month’s webinar will focus on BitCurator and metadata output, including the following topics:

Metadata produced byt the image capture process
File system metadata
An overview of DFXML and export capabilities
PREMIS event system metadata
How BitCurator-generated metadata fits into your archival workflow
There are no prerequisites for this webinar; however, it is designed for users already familiar with the basic operations of the BitCurator environment. The webinar will be roughly one hour with 10 minutes for Q&A at the end.

### Bitcurator: Forensics for Collecting Institutions (Part 1 of 2) (originally published March 5, 2014)

Part one of two guest posts by Kari R. Smith of the Massachusetts Institute of Technology Libraries, Institute Archives and Special Collections. Cross-posted from the Engineering the Future of the Past blog (CC BY-SA 3.0).

We’ve been busy the past few months.  Take the blog silence for the quiet of busy beavers rather than the absence of activity!

Photo of BitCurator Project Sticker
BitCurator Project Sticker
As noted in the workflow diagrams, one of the tools that we are assessing both in terms of functionality and how it might fit into our workflows is BitCurator.  The BitCurator Team has lot of information on their project and release portal pages that you should read to keep current on this Mellon funded project.

Photo of the BitCurator in a Box. Includes two write-blockers, cables and cords, and BitCurator program on a USB drive
Photo of the BitCurator in a Box. Includes two write-blockers, cables and cords, and BitCurator program on a USB drive
The BitCurator Project is an open-source digital forensics environment in which collecting institutions can create and analyze forensic disk images of digital content, whether from a file server or from media.  Read this page on the BitCurator website for more specifics on the projects and the tools incorporated into the environment.

We’ve been testing versions of the BitCurator tools since version 3.0.  Happily, the project and team have been doing great work with adding tools, functionality, GUI, and reporting capabilities.  BitCurator 0.7.4 was released on February 2, 2014 and is the current version we are assessing.

As an activity of the Digital Sustainability Lab in the Libraries, there is input into the assessment from both the Institute Archives and Special Collections staff and from the Digital Curation and Preservation staff in the MIT Libraries.

The BitCurator team is fantastic and are very responsive to feedback and questions regarding how to use and implement BitCurator in your digital curation workflow.  For instance, at the recent DigCCurr Institute, CurateGear presentations it came up that there was a BitCurator in a Box that can be borrowed for formal assessment purposes.  We asked and after the most current release at that time we were mailed the box.  Along with a formal testing plan and required questions/ answers to return to the BitCurator Team, was a jumpdrive with the BitCurator install files and two write-blockers with accompanying cables and cords. It is all packed into a Pelican case for shock absorption and a cool factor.

The next blog post on this topic will frame our assessment and the issues and considerations that we are addressing.

### BitCurator This Week (February 24th) (originally published February 24, 2014)

The BitCurator team will be participating in a number of outreach activities this week, including talks by Cal Lee at the Personalized Access to Cultural Heritage (PATCH) conference, Alex Chassanoff at the International Digital Curation Conference (IDCC 2014), and Porter Olsen at MITH’s Digital Dialogues lecture series. Details for each are listed below. Check back next week for follow-up posts on each of the different venues.

Cal Lee

“Up Close and Personal: Individual Digital Traces as Cultural Heritage and Discovery through Forensics Tools”   PATCH 2014–Monday, Feb. 24th at 10:30 IST.

Alex Chassanoff

“Integrating digital forensics techniques into curatorial tasks: A Case Study” with Sam Meister of the University of Montana. IDCC 2014–Wednesday, Feb. 26th at 3:00pm PST.

Porter Olsen

“What Falls Out: Preserving our Digital Heritage with BitCurator.” MITH Digital Dialogues–Tuesday, Feb. 25th at 12:30 EST.

### BitCurator 0.7.4 Now Available (originally published February 18, 2014)

The latest release of the BitCurator environment (0.7.4) is now available on our Release page (https://github.com/BitCurator/bitcurator-distro/wiki/Releases). We’re continuing to provide download options on our existing host and via iBiblio. Direct links and MD5 checksums can be found on the Release page.

This release includes the following updates:

– The mounting scripts have been fixed to mount disk images – without asking for authentication – from all locations.
– The desktop now includes a folder named “Shared Folders and Media” that points to the /media directory. When users adds a host shared folder, it will automatically appear in this location with an “sf_”  prefix.
– ClamTK is now linked in the Additional Tools folder.
– The filint tool is also now linked in the Additional Tools folder as a convenience for keeping the VM clean.
– The ficlam scripts, which run ClamAV scans during a fiwalk run, are now in the /Tools/ficlam directory, and there is a slide showing how to run them in the Quickstart guide.
– A dd command-line launcher has been added to the Imaging Tools directory

Our updated Quickstart guide can be found in the Documentation folder on the BitCurator environment desktop.

As with previous releases, this environment is built on a 64-bit version of Ubuntu and may be unstable on certain 32-bit host operating systems, or host hardware with less than 4GB of RAM. Please don’t hesitate to post here if you have questions!

### Call for Proposals: BitCurator On-Site Visit and Training (originally published February 7, 2014)


The BitCurator project has funds for a limited number of on-site BitCurator training and workshop visits. We are requesting proposals from collecting institutions (libraries, museums, and archives) who are interested in having a member of the BitCurator team visit their institution to conduct a workshop and/or provide hands-on training for archivists currently working with born-digital materials. Priority will be given to institutions who are already working with digital collections and wish to add BitCurator to their workflows.

About the BitCurator Project

BitCurator, funded by the Andrew W. Mellon Foundation, is a joint effort led by the School of Information and Library Science at the University of North Carolina, Chapel Hill (SILS) and the Maryland Institute for Technology in the Humanities (MITH) to develop a system for collecting professionals that incorporates the functionality of many digital forensics tools.

In Phase I (November 2011 – September 2013), the BitCurator team developed the BitCurator environment, a highly customized Linux distribution that includes both existing open source digital forensics tools and custom tools developed by the BitCurator team. The BitCurator environment stands out from other digital forensics environments (CAIN) and commercial software suites (FTK) in that it was designed specifically for use by memory institutions.

In Phase II of the BitCurator project (now ongoing) we are continuing to develop the BitCurator environment while simultaneously working to build a community of BitCurator users who will help sustain the project into the future.

Scope of Site Visits

Site visits are a chance for you to learn more about the use of digital forensics in digital curation and receive hands-on training from a member of the BitCurator team. Site visits might include visiting a library, museum, or archive, or attending an event such as a professional conference or workshop. We also welcome proposals to visit area institutions that may include any of the above.

There are three main objectives to the BitCurator site visits:

Educate digital curation practitioners (considered broadly) at the host institutions/events about the BitCurator project, its goals, and development thus far

Provide hands-on training in the BitCurator environment for one or more digital archivists at the host institutions/events

Work to develop digital curation workflows that include the digital forensics tools in the BitCurator environment

To achieve those goals, the BitCurator Community Lead, Porter Olsen, will visit the host institution for one to two days, depending on the pre-arranged itinerary.

Proposal Details

Please submit your proposal by emailing it to Porter Olsen at: polsen at umd do edu. Proposals should include the following information:

Name of the host or hosts (proposals involving multiple institutions in the same location are strongly encouraged)

Type and name of the host institution or event

Date on which you would like to host the visit

A brief description of existing digital curation efforts currently underway at your institution

The outcomes you would like to achieve as the result of a BitCurator site visit

Any opportunities for public demonstrations or discussions of BitCurator (ex: guest lectures, speaking engagements, workshops, etc.)

You may also wish to include details regarding the digital or hybrid collection(s) you are working with at your institution. Such details might include:

Name of the collection

Types of media in the collection

Hardware being use to process the collection

Current digital curation workflows

As noted, the BitCurator project has funding to cover travel and lodging at the host institution; however, cost-sharing is welcome, and may impact our ability to accommodate a given visit.

Submission Details

Please submit your proposal to Porter Olsen via email at: polsen at umd dot edu. Submissions will be reviewed on an ongoing basis, but all site visits must be conducted before September 15, 2014.

### BitCurator 0.7.0 Now Available (originally published February 2, 2014)

The latest release of the BitCurator environment (0.7.0) is now available on our Release page (https://github.com/BitCurator/bitcurator-distro/wiki/Releases). We’re continuing to provide download options on our existing host and via iBiblio. Direct links and MD5 checksums can be found on the Release page.

This release includes the following updates:

File Export tab added to GUI. This new tab runs fiwalk and uses the output to generate a tree-style hierachy of the file system in a new window. This allows you to safely navigate through directory and file contents and export file items without having to mount the file system.
Removes bugs affecting the operation of the fiwalk and annotation tabs in the BitCurator GUI.
Updates The Sleuth Kit to 4.1.3.
Now includes ClamTK, a graphical front-end to the Clam virus scanner. ClamTK simplifies the process of scanning mounted file systems and regular directory contents.
Our updated Quickstart guide can be found in the Documentation folder on the BitCurator environment desktop.

As with previous releases, this environment is built on a 64-bit version of Ubuntu and may be unstable on certain 32-bit host operating systems, or host hardware with less than 4GB of RAM.

### BitCurator Webinar Series: Working with External Media in BitCurator (originally published January 27, 2014)

Join us for our next webinar by registering here.

Date: Wednesday, February 19, 2014

Time: 11:00 AM to 12:00 PM (EST)

Before scanning for PII or analyzing a file tree, the digital archivist must first be able to read and transfer data from the original storage media to a long-term sustainable format. Accessing data on original media–especially for legacy media such as 5.25”, 3.5” and Zip disks–can often present a challenge and may require specialized hardware. This webinar covers the various methods and hardware tools required to capture forensic disk images from a wide variety of media types for use within the BitCurator environment. Topics covered will include:

An overview of media reader devices for legacy media, including the Kryoflux and FC5025 floppy drive controllers

Using media devices with BitCurator running as a virtual machine

How and why to use a write-blocker in digital acquisition

An introduction to the Forensics Recovery of Evidence Device (FRED), a computer system designed for the acquisition and imaging of a broad array of external and internal media, now frequently used by digital archivists in collecting institutions

There are no prerequisites for this webinar; however, it is designed for users already familiar with the basic operations of the BitCurator environment. The webinar will be roughly one hour with 10 minutes for Q&A at the end.

### BitCurator 0.6.2 Now Available (originally published January 24, 2014)

The latest release of the BitCurator environment (0.6.2) is now available at our Release site (https://github.com/BitCurator/bitcurator-distro/wiki/Releases). As of 0.6.2, iBiblio serves as our primary distribution site. There should be a noticeable improvement in download speeds, particularly for international users. Direct links and MD5 checksums can be found on the Release page.

This release includes the following updates:

– Removes a bug where raw disk images could not be processed via the GUI
– Updates reporting tool to accommodate recent changes in identify_filenames
– bulk_extractor upgraded to 1.4.4. This addresses a number of issues, including a base64-encoded data handling bug.
– Guymager upgraded to 0.7.3 — many improvements; see http://sourceforge.net/p/guymager/wiki/Guymager%200.7.x/
– Moves pre-release install scripts to a staging area

Our updated Quickstart guide can be found in the Documentation folder on the BitCurator environment desktop.

As with previous releases, this environment is built on a 64-bit version of Ubuntu and may be unstable on certain 32-bit host operating systems, or host hardware with less than 4GB of RAM. Please don’t hesitate to post here if you have questions!

## 2013 Posts

### BitCurator 0.5.8 Now Available (originally published December 20, 2013)

BitCurator environment (0.5.8) is now available at our Release site (https://github.com/BitCurator/bitcurator-distro/wiki/Releases).

This is a maintenance release that reduces the size on disk of the VM and ISO, eliminates an inaccurate error message on startup for some machines, and updates the VirtualBox extensions to 4.3.6.

Our updated Quickstart guide can also be found in the Documentation folder on the BitCurator environment desktop.

As with previous releases, this environment is built on a 64-bit version of Ubuntu and may be unstable on certain 32-bit host operating systems, or host hardware with less than 4GB of RAM. Please don’t hesitate to post here if you have questions!

### BitCurator Webinar on bulk\_extractor, fiwalk, and the BitCurator Reporting Tool (originally published December 11, 2013)

Our second in the BitCurator Webinar Series, this webinar builds on last month’s introduction to the BitCurator environment and offers a closer look at three of the main tools that comprise the BitCurator environment:

bulk\_extractor and BEViewer: digital forensics tools that can locate personally identifiable information (PII) and other types of sensitive data on a disk image
fiwalk: a digital forensics tool that processes a disk image using the SleuthKit library and outputs its results in Digital Forensics XML
The BitCurator Reporting Tool: BitCurator’s graphical interface for running the above tools and producing the BitCurator reports
The webinar will be held from 11:00 AM – 12:00 PM (EST). Please register in advance here: http://bitcurator-dftools.eventbrite.com

While there are no prerequisites for this webinar, it is designed for users already familiar with the basic operations of the BitCurator environment. The webinar will be roughly one hour with 10 minutes for Q&A at the end.

To learn more about BitCurator, please visit the main BitCurator page at bitcurator.net. You are also invited to join the BitCurator users group, join our facebook group, and follow us on twitter at @BitCurator.

### New White Paper from the BitCurator Team on Putting Digital Forensics into Practice in Collecting Institutions (originally published November 26, 2013)

The BitCurator team is pleased to announce the availability of the BitCurator Phase I white paper, From Bitstreams to Heritage: Putting Digital Forensics into Practice in Collecting Institutions. The press release announcing the white paper can be read below and also on the SILS website at: http://sils.unc.edu/news/2013/bitcurator-white-paper

From Bitstreams to Heritage: Putting Digital Forensics into Practice in Collecting Institutions

Out of the blue, an archivist gets a call from the husband of a famous scientist who has recently passed away. He wants to donate materials to the archives that can help people to understand and learn about her research. The archivist visits their home and is handed a cardboard box. Inside are not sheets of paper but a stack of floppy disks, CDs, Zip disks and a hard drive. What’s the archivist to do?

Researchers at the School of Information and Library Science (SILS) at the University of North Carolina at Chapel Hill, and the Maryland Institute for Technology in the Humanities (MITH) at the University of Maryland are investigating methods and developing tools for these sorts of situations.

A new white paper titled, “From Bitstreams to Heritage: Putting Digital Forensics into Practice in Collecting Institutions” examines the application of digital forensics methods to materials in collecting institutions – particularly libraries, archives and museums. It is a product of the BitCurator project and is written by Drs. Christopher A. Lee, Frances Carroll McColl Term Professor and research associate, Kam Woods of SILS; Matthew Kirschenbaum, associate director of MITH; and SILS doctoral student Alexandra Chassanoff.

”The landscape has changed quite dramatically in the past few years,” said Lee. “The white paper reflects a great deal of energy and progress around the work of extracting, securing and describing information that’s been stored on computer disks and drives.”

The BitCurator project, funded by the Andrew W. Mellon Foundation, is “an effort to build, test and analyze systems and software for incorporating digital forensics methods into the workflows of a variety of collecting institutions.” Procedures and tools for acquiring and validating data from physical media are well established in the field of digital forensics. There is a rich and growing body of open source tools that can be used to process, manage and disseminate forensically acquired data. While the primary target for many of these tools and methods is the law enforcement community, there is great potential for connecting these two streams of activity in order to support the work of collecting institutions.

BitCurator is developing and disseminating a dedicated open-source software environment that can be used to apply digital forensics methods to collections. The software and associated guidance documents are freely available on our Release page: https://github.com/BitCurator/bitcurator-distro/wiki/Releases

According to the white paper, “Forensic methods identify, capture and retain various forms of contextual information, which can be vital for users making meaningful use of digital materials.” It explains those processes, along with many associated challenges and opportunities

“BitCurator now moves into a critical next phase, with a full-time dedicated Community Lead based at MITH whose mandate is outreach to collecting institutions,” said Kirschenbaum. “We look forward to working with a wide variety of archives, special collections, museums and other constituencies to create a robust user community around our platform.”

The white paper is now available at: https://bitcurator.net/wp-content/uploads/sites/1099/2018/08/bitstreams-to-heritage.pdf

### Cal Lee on WREK Atanta’s “Lost in the Stacks” Radio Show and Podcast (originally published November 26, 2013)

Listen to BitCurator PI Cal Lee address the need for digital preservation on WREK Atlanta’s “Lost in the Stacks” radio show and podcast, the “one-and-only research-library rock’n’roll radio show!” Cal addresses the long-term sustainability of digital media, various approaches to digital preservation, and the aims of the BitCurator project–all while surrounded by an eclectic radio mix of songs dealing with “Bad luck and trouble.”

Listen here: http://lostinthestacks.libsyn.com/bit-rot  (Click on the “POD” button).

### Announcing the BitCurator Webinar Series (originally published November 1, 2013)

We are happy to announce the first in our BitCurator webinar series: An Introduction to the BitCurator Environment. This webinar will be the first in a monthly series of webinars addressing the use of Digital Forensics in the curation of born-digital materials. It will take place on Wednesday, November 20th from 10:00am – 11:00am EST and again from 2:oopm – 3:00pm EST. We will introduce participants to the basic functions of the BitCurator environment–from installation to generating forensics metadata reports. Specific topics covered will include:

Installing BitCurator as either a virtual machine or a stand-alone operating system
Learning to navigate within the BitCurator environment (BitCurator is a modified version of Ubuntu Linux)
Working with external media within BitCurator
Creating disk images via Guymager
Searching a disk image for personally identifiable information (PII)
An introduction to DFXML (Digital Forensics XML)
Generating the BitCurator reports
To attend this webinar, please register here in advance for the session you would like to attend by clicking on the appropriate link below.

Session One beginning at 10:00am EST

Session Two beginning at 2:00pm PST


We are limiting each webinar to 30 participants, so we encourage you to register early.  If you have any questions about the event, please contact Porter Olsen at polsen at umd dot edu.

### BitCurator 0.4.0 Release (originally published October 14, 2013)

Announcing BitCurator version 0.4.0!

BitCurator 0.4.0 includes significant improvements in the processing times required to analyze a forensics disk image. In addition, the BitCurator Reporting Tool interface has been updated to be more intuitive and now includes a “Run All” option that will generate DFXML outputs, annotate Bulk Extractor features, and create the BitCurator human and machine readable reports all as one action.

We invite you to download the latest BitCurator release, either as a virtual machine or installable ISO image, from the Release page, where you can also find documentation and a link to our BitCurator users group.

BitCurator 0.4.0 Change Log:

Bitcurator Reporting Tool and GUI now includes “Run All” tab. This provides a link to launch BEViewer, and a single form in which fiwalk, the annotation tool, and the reporting tools can be run.
Significant performance improvements in Bulk Extractor, fiwalk, and the BitCurator reports generation.
Excel report generation now handled by XlsxWriter 0.4.3; major performance improvements.
Bulk extractor updated to 1.4.1. Bug fixes and UI enhancements in BEViewer.
Sleuthkit updated to 4.1.2.
BitCurator report configuration (install location: /etc/bitcurator/bc-report-config.txt) updated to automatically report on system files. Various bug fixes.

### BitCurator Visits SAA 2013 (originally published August 19, 2013)

Last week, members of the BitCurator team visited New Orleans for the 2013 Society of American Archivists (SAA) Joint Annual Meeting. On Tuesday, August 13, we presented a poster at the 7th Annual SAA Research Forum on how the BitCurator environment can support archivists’ preservation goals in institutions.

In our poster, we described four preservation scenarios during the creation and ingest of a disk image into an archival repository. We then showed how the output generated by BitCurator tools during each scenario can be captured and stored as PREMIS-encoded preservation events.

Event 1: Image Capture
Definition: A forensic disk image is extracted from the original media source and created.
Tool: Guymager
Metadata: Acquisition time; duration of capture; manufacturing device & serial number; user who performed acquisition; cryptographic hash values

Event 2: File System Analysis
Definition: A set of file-objects corresponding to all of the files and directories identified on a disk image is analyzed and reported.
Tool: fiwalk
Metadata: Time of analysis; duration of analysis; user who performed file system analysis; file system partitions; file system volumes

Event 3: Feature Analysis
Definition: Describes forensic analysis of the raw bitstream, producing reports on specific features of interest (such as personally identifying or other sensitive information).
Tool: bulk extractor
Metadata: Time of analysis; execution environment; number of reports produced;

Event 4: Redaction
Definition: Used to overwrite specific patterns within the disk image according to a user-supplied rule-set.
Tool: iRedact.py
Metadata: Time of redaction; environment details; user performing redaction; name of new redacted image

### Building a Digital Curation Workstation with BitCurator (update) (originally published August 2, 2013)

*Original post by Porter Olsen. Minor edits in July 2018 to resolve broken links and media.*

Last year I wrote a post for the MITH blog describing how to build a digital curation workstation using readily available hardware (at least for the present) and the BitCurator suite of digital forensics tools. Matt Kirschenbaum and I revisited that topic a few weeks ago for a poster we presented at the Digital Humanities 2013 conference. We got a number of requests asking for the digital version of the poster, so I’ve revised it slightly and uploaded the poser in blog form below.

The most significant update from my orginal post in 2012 is the case study involving the transcription work done by Niel Fraistat on Percy Shelley’s Prometheus Unbound manuscripts–completed in 1989 and saved on 5.25″ floppy disks. Otherwise much of the information remains the same, though there is significantly more detail regarding the BitCurator suite of tools. As always, feel free to leave questions or comments in the Comments section below.

Introduction

This post builds on the recent report from the Online Computer Library Center (OCLC) titled “You’ve Got to Walk Before You Can Run: First Steps for Managing Born-Digital Content Received on Physical Media” (Erway, 2012).  The OCLC report identifies eleven specific steps archivist can follow to safely and effectively process born-digital content. This post considers the hardware needs of archivists and scholars as they look to implement the OCLC’s recommendations by offering a model born-digital curation workstation using readily available PC hardware and a suite of free and open source tools being developed and extended by the BitCurator project. We also demonstrate why such a workstation would be a valuable asset for a working digital humanities center through a case study involving the Shelley-Godwin Archive.

About BitCurator

BitCurator is a research and open source software development project designed to bring digital forensics tools and techniques to collecting institutions.

The BitCurator Environment is a Linux based suite of digital forensics tools that facilitate the creation of forensic disk images, file analysis, meta data extraction, and the identification of personally identifiable information (PII). BitCurator can be installed as either a stand-alone Linux operating system or as a virtual machine within a Windows or OS X host.

“Standard” Hardware

While there exist custom hardware solutions for preserving digital content, these options can be cost prohibitive, especially for a smaller DH center. For example, the Forensic Recovery of Evidence Device, or FRED, from Digital Intelligence can cost several thousand dollars. By contrast, the workstation we demonstrate here is designed to cost just over a thousand dollars, including the media access devices described in the next section.

The workstation will begin with a standard Windows or OS X based PC. While the exact technical specifications can vary, we offer the following recommendations as the minimum specifications for a digital curation workstation. More powerful hardware will, of course, result in less processing time, but a computer system with the specifications below should be available for roughly $500 from any number of retailers.

A multi-core CPU such as the Intel i5 series or AMD Fusion line of CPUs. The digital forensics tools in the BitCurator environment are mulit-threaded, so they will take advantage of multiple CPU cores and thus speed up processing times. Older multi-core CPUs such as the Intel Core2 series can also function well with BitCurator. If running BitCurator as a virtual machine, make sure your CPU has support for hardware virtualization: VT-x on Intel CPUs, and AMD-V on AMD.

Four to Eight Gigabytes of RAM. We recommend at least 4 gigabytes of RAM. BitCurator can run with less, but performance will suffer. 8 gigabytes of RAM is recommended if you plan to run BitCurator as a virtual machine within a host operating system.

Hard drive storage based on need. You will need at least 20 gigabytes of storage space to install BitCurator, beyond that you will want to plan for storage needs based on the media you will be accessioning.

Memory card reader and Blu-ray player. Choose a memory card reader with support for as many types of memory cards as possible. The Blu-ray player should be backwards compatible with burned DVDs and CD-ROMs.

Digital Curation Hardware

The hardware described below and shown in the image of our digital curation workstation allows the user to access a wide array of digital media. This is by no means an exhaustive list of media access devices, but it should be enough to handle most forms of legacy media and offer a starting point for those who may need more specialized hardware. (Pricing details are included to show the overall cost of the a digital curation workstation.)

USB 3.5” Floppy Disk Drive

Still available new from online retailers, look for a drive that can read both 1.44 MB(HD) and 800 KB (DD) 3.5” diskettes. Most drives support HD diskettes in both PC and Mac format, but only support PC formatted DD diskettes. Units are still available for around $20.

External USB 250MB Zip Drive

These units are available both new and used. We recommend the 250MB model as it is backwards compatible with the 100MB Zip disks. New units retail for around $200 and used units for around $50.

USB 250 MB Zip Drive and 3.5" Floppy Disk Drive
USB 250 MB Zip Drive and 3.5″ Floppy Disk Drive
Device Side Data’s FC5025

The FC5025 is a controller card for 5.25” floppy disk drives that can be used as an internal or external—as seen here—interface. Device Side Data charges $55.25 per controller.

FC5025 5.25" Floppy Drive Controller
FC5025 5.25″ Floppy Drive Controller
5.25” Floppy Disk Drive

These units are no longer available new, but can still be purchased off of eBay for about $50. Drives can be mounted in a PC case or used as external devices as shown in the digital curation workstation example below.

Because 5.25″ floppy drives are no longer manufactured, we recommend that you purchase a number of back up drives based on your need. We also recommend a disk drive cleaning kit.

Backup your capacity to backup
Backup your capacity to backup
Wiebetech UltraDock Hardware Write Protector

This unit serves as both an interface with IDE and Serial ATA  type hard disk drives and as a write protector. Because it is common for the OS to overwrite metadata on a hard drive, write protection ensures that no interactions of the archivist or researcher affects the integrity of the original media. Wiebetech charges $250 for the UltraDock Hardware Write Protector.

WiebeTech Forensic ComboDock Writer Blocker
WiebeTech Forensic ComboDock Writer Blocker
How Things Come Together

Digital Curation Workstation
Digital Curation Workstation
BitCurator Digital Forensics Tools

The BitCurator Environment includes 3rd-party  and custom tools for disk imaging, data triage, PII discovery, filesystem analytics and reporting, and metadata export. It incorporates scripted actions that can be run in the GUI against live filesystems for file analysis prior to (or in lieu of) imaging. Additionally, it includes unique software for producing human-readable reports from forensic tool output.

BitCurator currently includes the following tools:

Guymager: A GUI-based disk imaging program for capturing disk images in raw, E01, and AFF formats.

Bulk Extractor and Bulk Extractor Viewer: A stream-based forensics tool for extracting features of interest from disk images (including but not limited to private and individually identifying information) and associated GUI front-end.

Fiwalk: A tool for generating Digital Forensics XML output describing filesystem hierarchies contained on disk images.

The Sleuth Kit: Basis Technology’s open source digital forensics framework.

BitCurator Reporting Tools: Custom tools developed by the BitCurator team for generating metadata reports useful for archivists and digital-curation practitioners.

Sdhash: A “fuzzy hashing” file similarity finding tool.

Digital Forensics plug-ins for Ubuntu’s GUI file browser (Nautilus) that can identify file information, generate check sums, read files in hexadecimal format, and perform other file analysis tasks.

Case Study: Recovering the Shelley-Godwin Archive

The half-life of bits: The evolution of Niel Fraistat's transcription of Shelley's Prometheus Unbound manuscripts.
The half-life of bits: The evolution of Niel Fraistat’s transcription of Shelley’s Prometheus Unbound manuscripts.
In 1989, Neil Fraistat worked with the Bodleian Library in Oxford to produce a transcript of Percy Shelley’s Prometheus Unbound manuscripts. These handwritten manuscripts included notations, line-throughs, revisions, line counts and other edits that made them challenging to read. Fraistat transcribed each page using WordPerfect 4.2 and then created a photo ready print of each transcribed page. The subsequent publication included a facsimile of the original page next to Fraistat’s transcribed version, as seen in the image above.  Completed on an IBM PC of the era, Fraistat’s work was saved on 5.25” floppy disks.

In 2012, MITH began working on the Shelley-Godwin archive, using Fraistat’s publication of Shelley’s manuscripts as a model for the digital implementation using Shared Canvas. However, the original transcription work–that had also been vetted by the Bodleian–now existed on essentially unreadable media, and in a format no longer supported by contemporary word processors. By using the FC5025 seen above and a used 5.25” floppy disk drive, we were able to recover Fraistat’s original transcriptions and preserve Fraistat’s work by creating disk images of the 5.25: floppy disks. We then used Open Office to convert the files to a format readable by a present-day word processor. The now-readable files were then passed to the editors for TEI encoding, saving hours of repeat labor.

This case study not only shows the utility of a digital curation workstation, but also asks us to rethink the history of digital humanities. We argue that Fraistat’s early work of thinking through representing analog, handwritten text in a digital medium represents an early form of DH scholarship. At stake in the archival work demonstrated here is not only the preservation of born-digital objects generally, but the ability to examine the history of our own disciplinary practices.

Conclusions

It is our argument that for a relatively small investment—roughly a thousand dollars—a digital humanities center can avail itself of the tools required to preserve, archive, and investigate a wide variety of born-digital materials. The hardware interfaces described in this post work in conjunction with the BitCurator Environment’s suite of digital forensics tools to achieve those ends and facilitate the recommendations of the OCLC report cited in the introduction.

The Shelley-Godwin Archive case study demonstrates the need for these tools—both hardware and software—in the DH community itself. If Fraistat’s original transcription of the Shelley manuscripts are an early form of DH, as we contend, then we see that what’s at stake here is not simply the concern of archivists and libraries, but the history and legacy of our own practices. The disciplinary sensibilities that inform the digital humanities make the DH center a logical location for these discovery and preservation tools. Further, the capacities afforded by the tools described in this poster will further demonstrate the value of a DH center to host institutions.

Acknowledgements

The BitCurator project is funded through the Andrew W. Mellon Foundation. The principle investigator is Christopher Lee and the co-principle investigator is Matthew Kirschenbaum.

Erway, Ricky. “You’ve Got to Walk Before You Can Run: First Steps for Managing Born-Digital Content Received on Physical Media.” OCLC 2013.

Reside, Doug. “Digital Archeology: Recovering Your Digital History.” NYPL 2012.

### Marty Gengenbach selected for National Digital Stewardship Alliance Innovation Award (originally published June 20, 2013)

Marty Gengenbach has been selected as one of four recipients of the National Digital
Stewardship Alliance Innovation Working Group Innovation Awards for work he
completed while a student at UNC SILS and in support of the BitCurator project.

Selected in the category of “Future Steward,” Gengenbach is recognized for
the Gates Archive and his “work documenting digital forensics tools and
workflows, especially his paper, “The Way We Do it Here: Mapping Digital
Forensics Workflows in Collecting Institutions” and his work on the
DFXML tag library.

http://sils.unc.edu/news/2013/martin-gengenbach-innovation-award

### 8th International Workshop on Systematic Approaches to Digital Forensics Engineering – Call For Papers (originally published June 14, 2013)

Call for Papers

SADFE 2013
8th International Workshop on
Systematic Approaches to Digital Forensics Engineering
In collaboration with Hong Kong University, Hong Kong Information Security and Forensics Society; Hong Kong Center for Information Security and Cryptography and the Hong Kong Law and Technology Center
November 21-22, 2013
Hong Kong University, Hong Kong, Peoples Republic of China

right before the HTCIA (High Technology Crime Investigation Association)
Law Enforcement Cyber Security Training Conference
November 25-29, 2013

Important Date:
Paper Due Date: Jun 24, 2013 (anywhere in the world)
Acceptance Notification Date: August 15, 2013
Final Paper: October 1, 2013
Conference Date: November 21-22, 2013

We invite you to SADFE-2013, the eighth international conference on Systematic Approaches to Digital Forensic Engineering to be held in Hong Kong, China November 21-22, 2013.

Digital forensics engineering and the curation of digital collections in cultural institutions face pressing and overlapping challenges related to provenance, chain of custody, authenticity, integrity, and identity. The analysis and sustainability of digital evidence requires innovative methods, systems and practices, grounded in solid research and understanding of user needs.

SADFE-2013 investigates the application of digital forensic engineering expertise to advance a variety of goals, including criminal and corporate investigations, as well as documentation of individual and organizational activities. We believe digital forensic engineering is vital to security, the administration of justice and the evolution of culture.

Submissions: Submissions are made via Reg-Site

A Best Paper Award will be made for the final papers.

Topics:

We welcome previously unpublished papers on digital forensics and preservation as to civil, criminal and national security investigations for use within a court of law, the execution of national policy or to aid in understanding the past and digital knowledge in general.

We discuss digital forensic principles in new areas of the information society. We hope you consider submission for this international conference.

Potential topics to be addressed by submissions include, but are not limited to:

Digital Data and Evidence Management: advanced digital evidence discovery, collection, management, storage and preservation
Identification, authentication and collection of digital evidence
Extraction and management of forensic data/metadata
Identification and redaction of personally identifying information and other forms of sensitive information
Post-acquisition handling of evidence and the preservation of data integrity and admissibility
Evidence and digital memory preservation, curation and storage
Architectures and processes (including network processes) that comply with forensic requirements
Managing geographically, politically and/or jurisdictionally dispersed data artifacts
Data, digital knowledge, and web mining systems for identification and authentication of relevant data
Botnet forensics

Digital Evidence, Data Integrity and Analytics: advanced digital evidence and digitized data analysis, correlation, and presentation
Advanced search, analysis, and presentation of digital evidence
Cybercrime scenario analysis and reconstruction technologies
Legal case construction and digital evidence support
Cyber-crime strategy analysis and modeling
Combining digital and non-digital evidence
Supporting both qualitative and statistical evidence
Computational systems and computational forensic analysis
Digital evidence in the face of encryption
Forensic-support technologies: forensic-enabled and proactive monitoring/response

Forensics of embedded or non-traditional devices (e.g. digicams, cell phones, SCADA, obsolete storage media)
Forensic tool validation: methodologies and principles
Legal and technical collaboration
Digital forensics surveillance technology and procedures
“Honeypot” and other target systems for data collection and monitoring
Quantitative attack impact assessment
Comprehensive fault analysis, including, but not limited to, DFE study of broad realistic system and digital knowledge failures, criminal and non-criminal, with comprehensive DFE (malicious/non-malicious) analysis in theory, methods, and practices.

Forensic and digital data integrity issues for digital preservation and recovery, including
Technological challenges
Legal and ethical challenges
Economic challenges
Institutional arrangements and workflows
Political challenges and
Cultural and professional challenges

Scientific Principle-Based Digital Forensic Processes: systematic engineering processes supporting digital evidence management which are sound on scientific, technical and legal grounds
Legal/technical aspects of admissibility and evidence tests
Examination environments for digital data
Courtroom expert witness and case presentation
Case studies illustrating privacy, legal and legislative issues
Forensic tool validation: legal implications and issues
Legal and privacy implications for digital and computational forensic analysis
Handling increasing volumes of digital discovery

Legal, Ethical and Technical Challenges
The forensic, policy and ethical implications of
n The Internet of Things, The “Smart City,” “Big Data” or Cloud systems
New Evidence Decisions, e.g., United States v. Jones, _ U.S._ (2012) and United States v. Kotterman, _ F.3d _ (9th Cir. 2013)
Computational Forensics and Validation
Transnational Investigations/Case Integration under the Convention on Cybercrime of the Council of Europe
Issues in Forensic Authentication and Validation.

Submission:

SADFE-2013 follows standard IEEE submission standards with full papers to be submitted by the final due date.

Prospective authors are invited to submit original work not previously published or planned for presentation. Papers are reviewed on the basis that they do not contain plagiarized material and have not been submitted to any other conference at the same time (double submission). Follow these links to learn more:

IEEE Policy on Plagiarism

IEEE Policy on Double Submission

PLEASE NOTE: To be published in the Conference Proceedings an author of an accepted paper is required to register for the conference. Non-refundable registration fees must be paid prior to uploading the final IEEE formatted, publication-ready version of the paper. For authors with multiple accepted papers, one registration is valid for up to 3 papers. Accepted and presented papers will be published in the 2013 Conference Proceedings.

Paper submissions:

During the initial paper submission process via REG-SITE, it is the authors’ responsibility to ensure that the author list and the paper title of the submitted pdf file is an exact match to the author list and paper title on the REG-SITE registration page. Registration must include all co-authors, not just the submitting author. Failure to comply with this rule might result in your paper being withdrawn from the review process.

All submissions should be written in English with a maximum paper length of six (6) printed pages (minimum 10-point font) including figures, without incurring additional page charges.

Standard IEEE conference templates for for Microsoft Word US letter is here: US letter.

Only PDF files will be accepted for the review process, and all submissions must be done through REG-SITE.

Steering Committee:

Deborah Frincke, Co-Chair (Department of Defense)
Ming-Yuh Huang, Co-Chair (Northwest Security Institute)
Michael Losavio (University of Louisville)
Alec Yasinsac (University of South Alabama)
Robert F. Erbacher (Army Research Laboratory)
Wenke Lee (George Institute of Technology)
Barbara Endicott-Popovsky (University of Washington)
Roy Campbell (University of Illinois, Urbana/Champaign)
Yong Guan (Iowa State University)

Organizing Committee:
General Chair: K.P. Chow, Hong Kong University
Program Committee Co-Chairs: Christopher (Cal) Lee, University of North Carolina
Adel Elmaghraby, University of Louisville
Submission Chair: Luciana Duranti, University of British Columbia

Program Committee:

Sudhir Aggarwal Florida State University
Galina Borisevich Perm State University
Long Chen Chongqing University of Posts and Telecommunications
K.P. Chow University of Hong Kong
David Dampier Mississippi State University
Hervé Debar France Telecom R&D
Barbara Endicott-Popovsky University of Washington
Robert Erbacher Northwest Security Institute
Xinwen Fu UMass Lowell
Simson Garfinkel Naval Postgraduate School
Brad Glisson University of Glasgow
Yong Guan Iowa State University
Barbara Guttman National Institute for Standards and Technology (USA)
Brian Hay University of Alaska, Fairbanks
Jeremy John British Library
Ping Ji John Jay College Of Criminal Justice
Yu-Li Li Ministry of Justice Investigation Bureau, Taiwan
Pinxin Liu Renmin University of China Law School
Michael Losavio University of Louisville
Nasir Memon Polytechnic Institute of NYU
Mariofanna Milanova University of Arkansas at Little Rock
Kara Nance University of Alaska, Fairbanks
Ming Ouyang University of Louisville
Gilbert Peterson Air Force Institute of Technology
Slim Rekhis University of Carthage
Golden Richard University of New Orleans
Corinne Rogers University of British Columbia
Ahmed Salem Hood College
Clay Shields Georgetown University
Vrizlynn Thing Institute for Infocomm Research, Singapore
Sean Thorp Faculty of Engineering and Computing at University of Technology , Jamaica
William(Bill) Underwood Georgia Tech
Wietse Venema IBM Research
Xinyuan(Frank) Wang George Mason University
Kam Woods University of North Carolina
Yang Xiang Deakin University, Australia
Fei Xu Institute of Information Engineering, Chinese Academy of Sciences
Alec Yasinsac University of South Alabama
SM Yiu Hong Kong University
Wei Yu Towson University
Nan Zhang George Washington University

Contact Information:
Michael Losavio, University of Louisville,
michael.losavio@louisville.edu
+1 502 852 3509

### Digital Forensics for Archivists – June 24-25, 2013 (originally published June 4, 2013)

Cal Lee and Kam Woods (Principal Investigator and Technical Lead for the BitCurator Project) will be offering the new two-day version of the Digital Forensics for Archivists class in Ann Arbor, Michigan on June 24-25, 2013.

http://saa.archivists.org/events/digital-forensics-for-archivists-1386/415/

This is part of the Digital Archives Specialist (DAS) curriculum for the Society of American Archivists. Learn about the fundamentals of digital forensics, application to archival workflows, and the latest capabilities of the BitCurator environment.

### OPF Hackathon (originally published May 13, 2013)

Do you have born-digital collections that you’re grappling with?  Old media with file-systems that you can’t read?  Concerns about disseminating your collections because they might contain sensitive information?  Have you created disk images but don’t yet have the ability to process that data on the images?

Or are you a developer who would like to tackle some real-world challenges that will directly benefit collecting institutions in caring for born-digital materials?  Are you adept at developing and applying open-source software and would like to learn through hands-on experience how to apply various open-source digital forensics tools to collections?

If you answered “yes” to any of the above, then we have an event for you!

The Open Planets Foundation and the University of Chapel Hill’s School of Library and Information Science proudly presents:

The OPF Hackathon at UNC Chapel Hill:
Tackling Real-World Collection Challenges with Digital Forensics Tools and Methods
Monday, June 3rd-Wednesday, June 5th
Registration cost: $150 (REDUCED!)
* includes 3 lunches and 2 dinners

Come join world renowned digital preservation experts, collection managers, and coders as we collectively hack through digital preservation problems using a variety of digital forensics methods and approaches.

Our expert facilitators will be available to provide hands on guidance.    We will also be presenting awards for best collection challenge and best technical solution!

This is the first OPF Hackathon taking place in the United States and we are thrilled to host you as we hack out solutions to common problems in born-digital collections.

Event information: http://bit.ly/Z09fls
Registration page: http://bit.ly/XK4zel

### DFXML Tag Library (originally published February 6, 2013)

We’re excited to announce the newest release of the DFXML TAG library,  which contains tags for all fiwalk-generated output.  The next release will contain tags for bulk extractor technical metadata and some additional file system metadata.  Special thanks to Marty Gengenbach, now the Electronic Records Archivist at the Kansas Historical Society, who began compiling the TAG Library as a master’s student at UNC SILS.

## 2012 Posts

### Mapping Digital Forensics Workflows in Collecting Institutions (originally published November 20, 2012)

Gengenbach, Martin J. “‘The Way We Do it Here”’ Mapping Digital Forensics Workflows in Collecting Institutions.” A Master’s Paper for the M.S. in L.S degree. August, 2012.

*This paper presents the findings of semi-structured interviews with archivists and curators applying digital forensics tools and practices to the management of born-digital content. The interviews were designed to explore which digital forensic tools are in use, how they are implemented within a digital forensics workflow, and what further challenges and opportunities such use may present. Findings indicate that among interview participants these tools are beneficial in the capture and preservation of born-digital content, particularly with digital media such as external hard drives, and optical or floppy disks. However, interviews reveal that metadata generated from the use of such tools is not easily translated into the arrangement, description, and provision of access to born-digital content.*

See especially Marty’s descriptions and graphical representations of the institutions’ workflows (pages 27-69).

### An Early Look at the BitCurator Environment (originally published October 25, 2012)

*The following blogpost was written by Porter Olsen, BitCurator’s Research Assistant at the Maryland Institute for Technology in the Humanities (MITH).*

Roughly one year ago members of the BitCurator Professional Experts Panel (PEP) met at MITH to help further refine the scope and priorities of the BitCurator project, and ensure that our efforts would have “real world” usefulness for archivists and librarians who are responsible for born-digital materials. The PEP meeting, along with a similar meeting in January of the Development Advisory Group, produced two significant results: first, revisions to a product requirements document that outlined the work to be done on the BitCurator project, including an architecture overview and feature descriptions; and second, a collection of detailed workflows that have helped us to identify where BitCurator can best fit into and enhance curatorial practices. The upcoming one-year anniversary of these initial meetings makes this a good time to take a look at how the BitCurator project has progressed and where we’re headed in the near future.

The BitCurator development team is making available at test release of the BitCurator Environment, which can now be downloaded from the Releases page. The BitCurator Environment is a fully functioning Linux system built on Ubuntu 12.04 that has been customized to meet the needs of archivists and librarians, and it can be run either as a stand-alone operating system or as a virtual machine. Once installed, the BitCurator Environment includes a number of digital forensics tools that can be integrated into digital curation workflows. A sampling of those tools includes:

Guymager: a tool for creating disk images in one of three commonly used disk image formats (dd, E01, and AFF).
custom Nautilus scripts: A collection of enhancements to Ubuntu’s default file browser that allow users to quickly generate checksums, identify file types, safely mount drives, and more.
bulk_extractor: a tool that locates personal identifiable information (PII) and then generates reports on that information in both human and machine readable formats.
Ghex: an open source hex editor that allows users to view a file in hexadecimal format.
The BitCurator environment will make additional available tools available in later releases.

The BitCurator team has also been developing various forms of documentation to complement the product development. On the BitCurator wiki you can find documentation that introduces virtual machines, instructs users on how to install the BitCurator environment, and gives detailed configuration instructions on sharing devices and files between host and virtual machines. We are also currently working on developing documentation that outlines use-case scenarios for digital archivists using the tools mentioned above.

It is not enough, of course, to simply build tools and a wiki page and hope users will come find our software. The BitCurator team has also been actively promoting the BitCurator Environment through lectures, panel discussions, conference talks, posters, and publications. Recent examples include presentations from Kam Woods (BitCurator technical lead), Cal Lee and Matthew Kirschenbaum (BitCurator Co-PIs) on BitCurator and digital forensics at this year’s Society of American Archivists conference in San Diego; and presentations by Cal at Archiving 2012 in Copenhagen, Denmark, Memory of the World in the Digital Age in Vancouver, Canada, the International Congress on Archives in Brisbane, Australia, and to the staff of the National Library of Australia in Canberra. In addition, team members Alex Chassanoff and Porter Olsen will present a poster on integrating digital forensics into born-digital workflows at the upcoming ASIS&T conference. We have also recently published an article in D-Lib Magazine titled “BitCurator: Tools and Techniques for Digital Forensics in Collecting Institutions.”

We have also been incorporating BitCurator elements into professional education offerings.  Cal has developed a one-day continuing education course called “Digital Forensics for Archivists” as part of the Digital Archives Specialist (DAS) curriculum of the Society of American Archivists (SAA).  Matt Kirschenbaum and Naomi Nelson (BitCurator PEP member) have been offering a course called “Born-Digital Materials: Theory & Practice” as part of the Rare Book School (RBS) at the University of Virginia.  Both the SAA and RBS courses serve as excellent mechanisms for raising awareness about BitCurator’s offerings and eliciting needs and perceptions from working professionals.

These are just a few examples of the work done by the BitCurator team to get the word out about BitCurator and our work on bringing digital forensics tools and techniques the digital curation community. For a full list of BitCurator related publications and presentations, please visit our project website at www.bitcurator.net.

As we look forward into the next few months, the BitCurator team has a number of goals and benchmarks that we will be working towards, chief among them being the release of the BitCurator beta later this fall. We are also organizing the second annual meeting of our Development Advisory Group for January 2013, where we will elicit feedback from DAG members on our releases to date. The day before the DAG meeting will be CurateGear 2013 on January 9 in Chapel Hill, where members of the DAG and many other experts will give presentations and run demos of software to support digital curation  And finally, we are currently in the process of applying for funding for phase two of the BitCurator project to support additional product development and further efforts to engage with working professionals who could benefit from implementation of the BitCurator tools. We invite those who are interested, especially those in collecting institutions working with born-digital materials, to follow our progress at www.bitcurator.net, or follow us on Twitter.  For those who would like to jump right in and start working with the BitCurator Environment, you can do so at the Release page and join theBitCurator Users List.

If you have questions about the BitCurator project or the role of digital forensics methods in born-digital curation, please feel free to ask them in the comments section below.

### ASIST 2012 Poster (originally published October 24, 2012)

Here’s a sneak preview of the BitCurator poster we’ll be presenting at ASIST 2012 in Baltimore this coming weekend/next week.   The poster reports on results obtained in the first year of the project which include: (1) detailed workflows documenting the handling of born-digital content in several collecting institutions; (2) specifications on how BitCurator can support the implementation of digital forensics tools and methods in curatorial workflow.

Poster: Integrating Digital Forensics into Born-Digital Workflows: The BitCurator Project

### CurateGear 2013: Enabling the Curation of Digital Collections (originally published October 24, 2012)


http://ils.unc.edu/digccurr/curategear2013.html

CurateGear 2013: Enabling the Curation of Digital Collections

January 9, 2013, 8:00AM-5:00PM
University of North Carolina at Chapel Hill
William and Ida Friday Center for Continuing Education

CurateGear 2013 is an interactive day-long event focused on digital curation tools and methods. See demonstrations, hear about the latest developments, and discuss application in professional contexts. This event is sponsored by Institute of Museum and Library Services, University of North Carolina School of Information and Library Science and The Andrew W. Mellon Foundation.

Register for CurateGear 2013

CurateGear 2013 Agenda

Symposium Speakers

Jonathan Crabtree, Odum Institute for Research in Social Science
Mark Evans, Tessella
Lisa Gregory, State Library of North Carolina
Barbara Guttman, National Institute of Standards and Technology
Carolyn Hank, McGill University
Chien-Yi Hou, University of North Carolina
Greg Jansen, UNC Libraries
Leslie Johnston, Library of Congress
Cal Lee, University of North Carolina
Jerry McDonough, University of Illinois
Nancy McGovern, MIT Libraries
Richard Marciano, University of North Carolina
Mark Matienzo, Yale University
Courtney Mumma, Artefactual Systems
Trevor Owens, Library of Congress
David Pearson, National Library of Australia
Doug Reside, New York Public Library
Ryan Scherle, Duke University
Seth Shaw, University Archives, Duke University
Katherine Skinner, Educopia Institute
Mike Thuman, Tessella
Helen Tibbo, University of North Carolina
William Underwood, Georgia Tech
Bram van der Werf, Executive Director, Open Planets Foundation
Doug White, National Institute of Standards and Technology
Kam Woods, University of North Carolina

### BitCurator 0.1.5 released (originally published September 12, 2012)

We’ve released BitCurator 0.1.5, which you can find on the Release page.

BitCurator 0.1.5 is an upgrade/maintenance release as we prepare to add reporting functionality in the next few weeks. Early reporting functionality will appear in 0.2, currently scheduled for mid-October. The current maintenance release includes updates to bulk extractor, scripting fixes for live data triage in Nautilus, and security patches.

Note that the virtual machine is now packaged as a .tar.gz file. Windows users will need a 3rd party file archiving utility such as 7zip to extract the VM.

### BitCurator requirements documents posted (originally published September 11, 2012)

Current versions of the BitCurator requirements documents have been posted. You can find them on the Release page.

These documents were originally prepared during the planning stages of BitCurator, and subsequently revised following feedback from our Professional Experts Panel and Development Advisory Group.

### Digital Forensics XML and Standardization (originally published September 9, 2012)

Wondering what the future of Digital Forensics XML looks like? You can find recent work by NIST at http://www.nsrl.nist.gov/Downloads.htm (with a draft schema from based on the original spec for fileobjects at http://www.nsrl.nist.gov/DFXML/fileobject.xsd). You can also find ongoing work as part of CyBOX at MITRE at http://cybox.mitre.org/.

BitCurator depends on DFXML output when producing reports on private and personally identifying information, disk and file formats and organization. As part of our commitment to identifying and implementing ways in which DFXML can be used to enhance the description of and provenance records associated with archival born-digital materials, we’ve joined in a discussion with NIST, MITRE, and other interested parties on the future of standards-compliant DFXML.

### BitCurator Requirements Document (v0.9) Available (originally published September 5, 2012)

This document contains the requirements for BitCurator development. Releases of this document following version 0.6 include information derived from current release and development materials documented at https://bitcurator.net/. Note that requirements for using BitCurator are located elsewhere.

### BitCurator welcomes Sunitha Misra to the team! (originally published August 2, 2012)

Sunitha Misra, Masters student in the UNC School of Information and Library Science, has joined the BitCurator team as a software developer for academic year 2012-2013. Welcome, Sunitha!

### Institutional Workflows (originally published May 16, 2012)

In December 2011 and January 2012, the core BitCurator project team met with advisory group members to elicit requirements for incorporating digital forensics tools and techniques into existing institutional workflows.

Based on the feedback we gathered, we’ve now drafted the steps for a BitCurator-supported workflow. We welcome additional feedback – please contact us.

### BitCurator in D-Lib Magazine (originally published May 15, 2012)

Read all about the BitCurator project, including current and ongoing development work, in the May/June 2012 edition of D-Lib Magazine:

BitCurator: Tools and Techniques for Digital Forensics in Collecting Institutions

### Bit By Bit: Recent Projects on Digital Forensics for Collecting Institutions (originally published January 24, 2012)

[Bit By Bit: Recent Projects on Digital Forensics for Collecting Institutions](http://blogs.loc.gov/digitalpreservation/2012/01/bit-by-bit-recent-projects-on-digital-forensics-for-collecting-institutions/)

The Signal, Library of Congress

January 24th, 2012 by Butch Lazorchak

*This is a guest post by Bradley Daigle, Director of Digital Curation Services and Digital Strategist for Special Collections, University of Virginia; Matthew Kirschenbaum, Associate Professor of English and Associate Director, Maryland Institute for Technology in the Humanities (MITH), University of Maryland; and Christopher (Cal) Lee, Associate Professor at the School of Information and Library Science at the University of North Carolina at Chapel Hill.*

## 2011 Posts

### BitCurator Poster at iDCC 2011 (originally published December 10, 2011)

The BitCurator project recently presented a poster at the International Digital Curation Conference in Bristol. You can check it out here!

BitCurator iDCC 2011 Poster

### CurateGear: Enabling the Curation of Digital Collections – January 6, 2012 in Chapel Hill (originally published November 2, 2011)

CurateGear: Enabling the Curation of Digital Collections
WHAT: The DigCCurr 2012 Public Symposium Presents CurateGear! a highly
interactive day-long event focused on digital curation tools and
methods. See demonstrations, hear about the latest developments, and
discuss application in professional contexts.

WHEN: Friday, January 6, 2012, 8:00 AM – 5:00 PM

WHERE: Friday Center, UNC, Chapel Hill, North Carolina

HOW TO REGISTER: Go to: http://tinyurl.com/3m8ajrm COST: $100 ($125 for
late registration beginning December 1st); STUDENT COST: $50.

Registration includes continental breakfast, morning and afternoon
breaks, lunch, and free parking.

### Events, how to follow BitCurator, and our upcoming press release (originally published September 24, 2011)

Information on BitCurator has begun to seep into the Twittersphere! If you’d like to keep track of our activity there, you can point your favorite client at our account.

You may see some project members at the OPF Hackathon this coming week… find us and say hello!

We’re working hard on an official press release. We’ll post it here as soon as it’s available.

Finally, if you’re curious about who’s involved, check out the updated project bios in the “People” tab above!

### BitCurator is alive! (originally published September 20, 2011)

BitCurator is a project to provide archivists, digital librarians, and content managers with tools and workflow enhancements drawn from (and developed in parallel with) the digital forensics community.

We will be spinning up project activities, software development, and event planning starting on October 1. For now, you can find basic project information, staff bios, and information on upcoming events in the main panel links.



