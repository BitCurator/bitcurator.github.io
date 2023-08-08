## BitCurator Project

The BitCurator project was a joint effort led by the School of Information and Library Science at the University of North Carolina, Chapel Hill (SILS) and the Maryland Institute for Technology in the Humanities (MITH) to develop a system for collecting professionals that incorporates the functionality of many digital forensics tools. The project was funded by [The Andrew W. Mellon Foundation](https://mellon.org) between 2011 and 2014 (grants [31100658](https://mellon.org/grants/grants-database/grants/university-of-north-carolina-at-chapel-hill/31100658/) and [11300659](https://mellon.org/grants/grants-database/grants/university-of-north-carolina-at-chapel-hill/11300699/). Ongoing maintenance and software development is managed by the [BitCurator Consortium](https://bitcuratorconsortium.org/).

BitCurator addressed two fundamental needs for collecting institutions absent from software designed for the digital forensics industry: incorporation into workflows of archives/library ingest and collection management environments, and provision of public access to the data. Two groups of external partners contributed to this process: a [Professional Expert Panel (PEP)](#professional-experts-panel) of individuals at various levels of implementing digital forensics tools and methods in their collecting institution contexts, and a [Development Advisory Group (DAG)](#development-advisory-group) of individuals who had significant experience with development of software.

BitCurator defined and tested support for a digital curation workflow that begins at the point of encountering holdings that reside on removable media—either new acquisitions or materials that are within a repository’s existing holdings—and extends to the point of interaction with an end user.

### Software

The BitCurator Environment is built on a stack of free and open source digital forensics tools and associated software libraries, modified and packaged for increased accessibility and functionality for collecting institutions. The BitCurator software is freely distributed under an open source license. It can be installed as a Linux environment; run as a virtual machine on top of most contemporary operating systems; or run as individual software tools, packages, support scripts, and documentation.

### Features of BitCurator include:

* Pre-imaging data triage
* Forensic disk imaging
* File system analysis and reporting
* Identification of private and individually identifying information
* Export of technical and other metadata

These tools are incorporated into the environment and workflow mapping in a modular fashion. Most are mature; as individual tools age, become deprecated, or lose support from upstream developers, they can be replaced without significantly altering the functionality of the environment.

Tools in the BitCurator Environment – both those produced by the project team and those from third-party developers – help advance core digital curation activities, including (but not limited to):

* Reducing the risk of inadvertent changes to content through software-based write-blocking
* Creating authentic copies of content through disk imaging and cryptographic hashing
* Mounting forensically packaged disk images to view & export contents
* Reflecting original order of materials through capture of file system metadata
* Establishing trustworthy chains of custody through documentation of curatorial actions (log files, PREMIS records)
* Generating reports that characterize the contents of disks and directories
* Identifying and documenting duplicate files
* Discovering and exposing associated contextual information
* Identifying sensitive information that should be filtered, redacted, or masked in appropriate ways
* Exporting contents of disks and directories for inclusion in Archival Information Packages and Dissemination Information Packages

# People

The personnel and advisory group bios here cover involvement between October 2011 and September 2014. They are retained for historical reference; current affiliations and positions may differ. Follow the bookmark links below to jump to personnel and advisory panel sections.

* [Project Personnel](#project-personnel)
* [Professional Experts Panel](#professional-experts-panel)
* [Development Advisory Group](#development-advisory-group)

## Project Personnel

### Christopher (Cal) Lee, PI (UNC SILS)

Christopher (Cal) Lee is Associate Professor at the School of Information and Library Science at the University of North Carolina, Chapel Hill. He teaches courses on archival administration; records management; digital curation; understanding information technology for managing digital collections; and acquiring information from digital storage media. He is a lead organizer and instructor for the DigCCurr Professional Institute, a week-long continuing education workshop on digital curation, and he teaches professional workshops on the application of digital forensics methods and principles to digital acquisitions.

Cal’s primary area of research is the long-term curation of digital collections. He is particularly interested in the professionalization of this work and the diffusion of existing tools and methods into professional practice. Cal developed [“A Framework for Contextual Information in Digital Collections,”](http://www.ils.unc.edu/callee/p95-lee.pdf) and edited and provided several chapters to [I, Digital: Personal Collections in the Digital Era](http://saa.archivists.org/4DCGI/store/item.html?Action=StoreItem&Item=2217&LoginPref=1) published by the Society of American Archivists.

Cal is Principal Investigator of the BitCurator project, which is developing and disseminating open-source digital forensics tools for use by archivists and librarians. He was also Principal Investigator of the Digital Acquisition Learning Laboratory (DALL) project, which investigated and tested the incorporation of digital forensics tools and methods into digital curation education. Cal has served as Co-PI on several projects focused on preparing professionals for digital curation responsibilities: Preserving Access to Our Digital Future: Building an International Digital Curation Curriculum (DigCCurr), DigCCurr II: Extending an International Digital Curation Curriculum to Doctoral Students and Practitioners; Educating Stewards of Public Information for the 21st Century (ESOPI-21), Educating Stewards of the Public Information Infrastructure (ESOPI2), and Closing the Digital Curation Gap (CDCG). In a project called Curation of a Forensic Data Collection for Education, Cal investigated and developed resources to enhance access and use of disk images to support digital forensics education.

### Matthew Kirschenbaum, Co-PI (MITH)

Matthew G. Kirschenbaum is Associate Professor in the Department of English at the University of Maryland and Associate Director of the [Maryland Institute for Technology in the Humanities](http://www.mith2.umd.edu/) (MITH, an applied thinktank for the digital humanities). He is also an affiliated faculty member with the [Human-Computer Interaction Lab](http://www.cs.umd.edu/hcil/) at Maryland, and a member of the teaching faculty at the University of Virginia’s [Rare Book School](http://www.rarebookschool.org/). His first book, [Mechanisms: New Media and the Forensic Imagination](http://mechanisms-book.blogspot.com/), was published by the MIT Press in 2008 and won the 2009 Richard J. Finneran Award from the Society for Textual Scholarship (STS), the 2009 George A. and Jean S. DeLong Prize from the Society for the History of Authorship, Reading, and Publishing (SHARP), and the 16th annual Prize for a First Book from the Modern Language Association (MLA). In 2010 he co-authored (with Richard Ovenden and Gabriela Redwine) [Digital Forensics and Born-Digital Content in Cultural Heritage Collections](http://www.clir.org/pubs/abstract/pub149abst.html), a report published by the Council on Library and Information Resources and recognized with a commendation from the Society of American Archivists. Kirschenbaum speaks and writes often on topics in the digital humanities and new media; his work has received coverage in the Atlantic, New York Times, National Public Radio, Wired, Boing Boing, Slashdot, and the Chronicle of Higher Education. He is a 2011 [Guggenheim Fellow](http://www.gf.org/). See [https://mkirschenbaum.wordpress.com/](https://mkirschenbaum.wordpress.com/) for more.

### Kam Woods, Technical Lead (UNC SILS)

Kam Woods is a Postdoctoral Research Associate in the School of Information and Library Science at the University of North Carolina at Chapel Hill. He is currently Technical Lead on the BitCurator project, and works with Dr. Cal Lee developing techniques and tools to assist in long-term archiving of born-digital data.

Kam’s research focuses on long-term preservation of born-digital materials. He is interested in interdisciplinary approaches that combine technologies and expertise in the areas of archiving, computer science, and digital forensics for the purpose of enabling and maintaining access to digital objects that are at risk due to obsolescence. Prior to his current work at UNC, Kam worked with Cal Lee on the development of educational materials to support the use of realistic forensic datasets in professional training and to identify and explore novel uses of forensic data and tools in the context of digital archives.

### Alex Chassanoff, Project Manager (UNC SILS)

Alex Chassanoff is a Ph.D. candidate in the School of Information and Library Science (SILS) at the University of North Carolina at Chapel Hill. Her research interests include the information behavior of digital archive users, digital materiality, and curation and preservation environments. Her current research looks at how historians use digitized photographs as evidence. Alex received her MSIS in 2009 and was a Digital Curation Fellow at SILS from 2008-2009. Prior to graduate school, she worked as a database programmer, IT consultant, and digital asset manager.

### Porter Olsen, Community Lead (MITH)

Porter is a Ph.D. candidate in the English Department at the University of Maryland. His research focuses on the intersections between postcolonial literature and digital cultures, with a particular interest in how both fields deploy virtual spaces as spaces of alterity. Before returning to graduate school, Porter worked as a product manager for a Linux distribution developer where he was a member of the United Linux initiative, an initiative designed to create a single Linux platform shared among distributors from Germany, Brazil, the U.S., and Japan.

### Sunitha Misra, Software Developer (UNC SILS)

Sunitha Misra is a Graduate Student at the School of Information and Library Sciences, pursuing her Masters in Information Sciences. She has a Masters degree in Computer Science from the University of Alabama in Huntsville. Prior to joining the SILS for her second Masters degree, she worked as a Software Developer for major Networking and Operating Systems companies in the San Francisco Bay area and in Research Triangle Park.

### Amanda Visconti, Graduate Research Assistant (MITH)

Amanda Visconti is a [MITH graduate research assistant](http://mith.umd.edu/people/person/amanda-visconti/) on the BitCurator project, where she creates user-friendly technical documentation, develops and designs for the web, and researches software usability. As a Literature Ph.D. candidate, she blogs about her digital humanities work regularly at [LiteratureGeek.com](LiteratureGeek.com).

### Kyle Bickoff, Graduate Research Assistant (MITH)

Kyle Bickoff is a Ph.D. candidate in the Department of English at the University of Maryland, College Park. His research focuses on electronic literature, net.art, and the archive’s role in relation to the curation and preservation of both printed and born-digital media.

Kyle received his M.A. in English Literature at the University of Colorado Boulder in 2014, where he worked at the Media Archaeology Lab (MAL) as Lab Manager and at the Archives and Special Collections Department for the University of Colorado Libraries where he preserved born-digital collections and maintained legacy hardware.

## Professional Experts Panel

### Bradley Daigle, University of Virginia Library

Bradley Daigle is Director of Digital Curation Services and Digital Strategist for Special Collections at the University of Virginia Library. He was also co-PI on a Andrew W. Mellon Foundation grant entitled “Born Digital Materials: An Inter-Institutional Model for Stewardship (AIMS).” Having been in the library profession for over a decade, he has published and presented on a wide range of topics including mass digitization, digital curation and stewardship, sustaining digital scholarship, intellectual property issues, mentoring in libraries, and digital preservation. In addition to his professional field, his research interests also include the history of the book, natural history, and early modern British literature. He received his MA in literature from the University of Montreal and an MLS from Catholic University.

### Erika Farr, Emory University

Erika Farr is the Coordinator for Digital Archives in the Manuscript, Archives, and Rare Book Library (MARBL) at Emory University in Atlanta, Georgia. She leads the born-digital archives program, assists with digitization projects, and supports other digital initiatives involving MARBL materials. She received her Master’s in Library Science from the University of North Texas at Denton and her Ph.D. in English Literature from Emory University. Her current research interests include human information behavior in archival settings and digital humanities research methodologies.

### Jeremy Leighton John, British Library

Dr. Jeremy Leighton John has been Curator of eMANUSCRIPTS and Scientific Curator in the Department of Western Manuscripts at the British Library since 2003, having been Specialist Curator for the W. D. Hamilton Archive from 2000. Previously he worked as a cataloguer of bioacoustic collections in the British Library Sound Archive. He served as Principal Investigator for Digital Lives, a major research project focusing on personal digital archives and their relationship with research repositories. In 1996 he completed a DPhil in Zoology at Merton College, Oxford. He is a member of the Library Committee of the Royal Society, and of the Advisory Committee of the National Cataloguing Unit for the Archives of Contemporary Scientists. He is also a Fellow of the Linnean Society of London and of the Royal Geographical Society, and is a member of the British Society for the History of Science. During his career, he has won several scholarships and prizes, including one for writing, has conducted both field and theoretical research, and has given talks and published articles on scientific, archival and historical topics, in both scholarly and popular forms. In recent years he has been working with hybrid (digital and analogue) collections of living as well as deceased scientists; and having first learned to program at University College London, with FORTRAN using punched cards, he has been adapting technologies and procedures for forensically capturing, authenticating and making available the digital equivalent of analogue personal archives and manuscripts.

### Leslie Johnston, Library of Congress

Leslie Johnston has over twenty years of experience in digitization and digital conversion, setting and applying metadata and content standards, and overseeing the development of digital content management and delivery systems and services. She is Chief of Repository Development in the Office of Strategic Initiatives at the Library of Congress. Previously, she served as the Manager of Technical Architecture Initiatives for the National Digital Information Infrastructure & Preservation Program at the Library; the Head of Digital Access Services at the University of Virginia Library; Head of Instructional Technology and Library Information Systems at the Harvard Design School; the Academic Technology Specialist for Art for the Stanford University Libraries; and as Database Specialist for the Getty Research Institute. Ms. Johnston has also been active in the museum community, working for various museums, teaching courses on museum systems, editing the journal Spectra, and serving on the board of the Museum Computer Network.

### Jennie Levine Knies, University of Maryland

Jennie Levine Knies is Manager, Digital Stewardship, at the University of Maryland Libraries. The University of Maryland’s Digital Stewardship initiative aims to provide a centralized project management base for digital projects, and to promote technology transfer throughout the University of Maryland Libraries. She is currently the principal investigator on the NEH-funded Historic Maryland Newspapers project (part of the National Digital Newspaper Program). A librarian since 1996, she has extensive experience with special collections and digital projects. Jennie received a bachelor’s degree and a Master’s of Library Science from the University of Maryland. She served as the chair of the EAD Roundtable of the Society of American Archivists from 2007-2008, and as the vice chair of the Mid-Atlantic Regional Archives Conference from 2007 to 2009. She has published on a variety of diverse topics, including historical research, Encoded Archival Description, and primary source literacy.

### Naomi L. Nelson, Duke University

Naomi L. Nelson is the Director of the Rare Book, Manuscript, and Special Collections Library at Duke University. She received a Masters in Library Science from the University of Pittsburgh in 1991 and a Ph.D. in History from Emory University in 2001. Her research interests center on managing and providing access to born-digital materials and on exploring the new avenues for humanities research opened by digital formats. She has been working with electronic records for over fifteen years, starting in 1996 when she served as a consultant to the Senate Computer Center on the transfer of born-digital Constituent Mail index files to archival repositories. She served on the Research Libraries Group’s Encoded Archival Description Advisory Group and on the Digital Library Federation’s Aquifer Initiative, consulted on the NDIIPP-funded MetaArchive initiative and on a Mellon-funded Digital Scholarship Planning grant, chaired the Society of American Archivists’ Technology Best Practices Task Force, and participated in a multi-institution NEH Digital Humanities Start-Up grant exploring approaches to collecting and managing born-digital literary materials. She has taught the Society of American Archivists’ courses “Digitization of Archival Materials” and “Digital Libraries and Digital Archives” and with Matt Kirschenbaum inaugurated the course “Born Digital Materials: Theory and Practice” at the University of Virginia’s Rare Book School. In a previous position at Emory University, she co-led the Libraries’ Born Digital Archives program that developed an innovative prototype researcher workstation demonstrating two ways to access the files from Salman Rushdie’s computers. While at Emory, she also co-directed the new graduate certificate program in Digital Scholarship and New Media.

### Erin O’Meara, Gates Archive

Erin O’Meara is an Archivist at the Gates Archive, where she manages digital strategy and the preservation of archival collections. The Gates Archive takes an innovative approach to archive development and management, integrating processes for born-digital and analog information. The archive focuses on the preservation of the Gates family’s personal and philanthropic endeavors including records of the Bill & Melinda Gates Foundation. From 2009-2011, she was the Electronic Records Archivist at the University of North Carolina at Chapel Hill where she helped deploy the Carolina Digital Repository. Before joining UNC Libraries, Erin served as the Electronic Records Archivist at the University of Oregon and as a NHPRC Electronic Records Research Fellow from 2006-2007, where she researched the recordkeeping practices of social scientists conducting data-intensive research. Erin received her Master of Archival Studies in 2004 from the University of British Columbia. While at UBC, she conducted research for the InterPARES 2 Project pertaining to archaeological records managed in a Geographic Information System.

### Michael Olson, Stanford University

Michael G Olson is a manager of digital projects for Stanford University Libraries. In this capacity he works with library curators and other non-library constituents to build and deliver digital collections, with a primary focus on unique special collections materials. Michael also works as a technology analyst for analog and electronic media and is currently leading efforts to migrate Stanford’s department of special collections and archive of record sound to the archivists’ toolkit.

Previous accomplishments include managing the Parker Library on the Web project during its first year, and processing many of Stanford’s born-digital collections, such as Robert Creeley’s Computer Files and the Stephen Cabrinety Collection of Computer Software that includes over five thousand software titles spanning 1974-94. Before joining Stanford University Libraries in 2001, Michael received an MPhil in History and Computing in 2000 from the University of Glasgow, and a BA from the University of British Columbia in Medieval Studies in 1997.

### Gabriela Redwine, University of Texas, Austin

Gabriela Redwine is Archivist and Electronic Records/Metadata Specialist at the Harry Ransom Center, where she is responsible for processing paper and born-digital collections, developing policies and procedures for the Ransom Center’s born-digital preservation program, and maintaining EAD versions of the Center’s finding aids. In 2010 she co-authored (with Matthew Kirschenbaum and Richard Ovenden) Digital Forensics and Born-Digital Content in Cultural Heritage Collections, a report published by the Council on Library and Information Resources (CLIR). She earned her MSIS and MA degrees from the University of Texas at Austin.

### Susan Thomas, University of Oxford

Susan Thomas is the Digital Archivist for the Bodleian Library’s Western Manuscripts department. She is responsible for developing the Library’s capacity to curate, preserve and provide access to born-digital archives. Susan has been involved in digital archives work – both projects and day-to-day work – for the past six years. She speaks and writes on the subject regularly, and undertakes a limited amount of related consultancy. Susan also serves on the Society of Archivists’ Data Standards Group Committee where, in the role of Training Officer, she helped to organize a series of regional road shows on digital preservation issues and tools during 2009/10.

Susan currently leads the futureArch project, an Andrew W. Mellon Foundation-sponsored initiative to develop and embed a sustainable approach to the curation of born-digital archives at the Library. This work includes the introduction of a service named ‘BEAM’ – Bodleian Electronic Archives and Manuscripts – to capture, store, preserve and provide access to digital archive material.

Previous projects include CAIRO (2006-8), a development project designed to facilitate initial processing of born-digital archives for submission to a digital preservation repository; and PARADIGM (2005-7), which explored digital preservation issues relevant to manuscript collections and collecting using the papers of politicians as sample collections.

Susan is also a member of the Data Standards Group Committee of the UK Society of Archivists, the UK team of the international interPARES3 project, the External Advisory Committee of the British Library’s Digital Lives project, and an Honorary Lecturer at the University of Dundee’s Centre for Archives Studies. Other digital preservation activities in which Susan has been involved include: the Computer Forensics and Cultural Heritage CLIR report (as a consultant); the iPres 2010 and 2011 Conference Programme Committees; and the Digital Lives Project Advisory Committee.

## Development Advisory Group

### Geoffrey Brown, Indiana University

Geoffrey Brown is a Professor of Computer Science at Indiana University, Bloomington. He received the BS in engineering from Swarthmore College, MSEE from Stanford University, and PhD from the University of Texas at Austin in 1987. He taught at Cornell from 1987-1997 and worked as a research scientist at Hewlett Packard Laboratories where he was one of the architects of the Lx (ST210) family of VLIW microprocessors, and architect at several networking start-ups. His research interests include verification and design of digital systems, and the preservation of digital documents.

### Barbara Guttman, National Institute of Standards and Technology

Barbara Guttman is the Manager of the Component Software Group in the Information Technology Laboratory (ITL) of the National Institute of Standards and Technology (NIST). In the position, she oversees the National Software Reference Library, the Computer Forensics Tool Testing Project and the Software Assurance, Metrics, and Tool Evaluation (SAMATE) Project. These projects address underlying issues of software identification and quality. She was a key member of the NIST Voting Team that produced the Voluntary Voting Systems Guidelines versions 1.0 and 2.0. Prior to this appointment, she worked in the ITL Laboratory Office as Associate Director for Federal and Industrial Relations, also serving as Acting Deputy Director and Acting Chief of the Statistical Engineering Division. She has also worked in the NIST Director’s office, serving first as the ITL Representative and then as the Senior Program Analyst to the Director. She started her career at NIST in computer security where she co-authored the NIST Computer Security Handbook and several other publications.

### Jerome McDonough, University of Illinois

Jerome McDonough is an Assistant Professor in the Graduate School of Library & Information Science at the University of Illinois. He is currently serving as the Principal Investigator for the Preserving Virtual Worlds project, a collaborative investigation into the preservation of computer games and interactive fiction being undertaken by Rochester Institute of Technology, Stanford University, the University of Maryland and the University of Illinois, and carried out under the Library of Congress’ National Digital Information Infrastructure for Preservation Program. Prior to joining the faculty at GSLIS, Dr. McDonough served as team leader for the digital library program at New York University. He has served as a member of NISO’s Standards Development Committee and has been involved in a variety of metadata standards initiatives, including METS, PREMIS and the Open Digital Rights Language. His research focuses on the application of metadata in digital library systems and the preservation of digital information.

### Mark Matienzo, Yale University

Mark A. Matienzo is Technical Architect for the ArchivesSpace project and a Digital Archivist in Manuscripts and Archives at the Yale University Library. He also teaches as an adjunct professor at the iSchool at Drexel (the Drexel University College of Information Science and Technology). His research and professional interests include digital curation, open source digital forensics, archival description, and media archaeology. In 2012, Matienzo was the first awardee of the Emerging Leader Award of the Society of American Archivists.

Prior to joining Yale University, he worked as an Applications Developer for the Digital Experience Group at The New York Public Library, as an assistant archivist at the Center for History of Physics at the American Institute of Physics, as an project cataloging archivist at the National Anthropological Archives, Smithsonian Institution, and as catalog librarian at ProQuest Information and Learning. He received his MSI from the School of Information at the University of Michigan and his BA in Philosophy from the College of Wooster.

### Courtney Mumma, Artefactual Systems

Courtney Mumma is responsible for managing Archivematica system requirements, product design, technical support, training, and community relations. She is a graduate of the University of British Columbia’s Master of Archival Studies and Master of Library and Information Studies programs (2009). Prior to joining Artefactual, Courtney worked at the City of Vancouver Archives implementing their digital archives system while managing the acquisition of the hybrid digital-analog 2010 Winter Olympic Games archives. She has been a researcher and co-investigator on the International Research on Permanent Authentic Records in Electronic Systems (InterPARES 3 Project), researcher on the UBC-SLAIS Digital Records Forensics Project, and a member of the Professional Experts Panel on the BitCurator Project. Courtney has been published in Archivaria and taught several workshops and delivered many presentations on the practical application of digital preservation strategies.

### David Pearson, National Library of Australia

David Pearson is currently acting Director of the Web Archiving and Digital Preservation Branch at the National Library of Australia (NLA). He has been involved in the development of digital preservation policy at both the strategic and technical level. He has developed a number of NLA concept papers and managed projects including the Mediapedia and Prometheus v1.0. During 2007, David was the NLA project manager for the Australian Partnership for Sustainable Repositories (APSR), a partnership between the NLA and a number of Australian universities. This collaboration produced two projects: the Australian METS Profile development project and the AONS II (Automatic Obsolescence Notification System, version II) project.

Before joining the Library, David designed, built and was subsequently the system manager of the first National Archives of Australia’s Digital Repository. He also supervised various data recovery projects involving hundreds of obsolete media carriers. Before this he worked in collection areas at the National Gallery of Australia and the Australian War Memorial [Museum].

David holds an honors degree in archaeology from the Australian National University, Canberra. He has written a number of articles in academic journals on both archaeological and digital preservation issues.

### Doug Reside, New York Public Library

Doug Reside became Digital Curator for the Performing Arts at New York Public Library in January of 2011 after serving for four and a half years on the directorial staff of the Maryland Institute for Technology in the Humanities (MITH) at the University of Maryland in College Park. He holds a BS in Computer Science and a BA, MA, and Ph.D. in English Literature. He has been a PI on three NEH startup grants (The Ajax XML Encoder, Music Theatre Online, and the Collaborative Ajax Modeling Platform) and the co-PI with Tanya Clement on the “Off the Tracks” workshop. Additionally, he is the original project director of the NEH Preservation and Access funded Text Image Linking Environment (TILE) which is scheduled for release in the summer of 2011.

### Seth Shaw, Duke University

Seth Shaw is the Electronic Records Archivist for Duke University Archives where he is responsible for everything born-digital in both the University Archives & Special Collections. He received his Bachelors of Science in Information Systems from Brigham Young University – Idaho in 2005 and his Masters of Science in Information, Archives & Records Management from the University of Michigan’s School of Information in 2007. Seth has taught workshops the Society of North Carolina Archivists (SNCA), South Carolina Archivists Association (SCAA), and Society of American Archivists (SAA) and has presented at SNCA, MAC, and SAA.

### William Underwood, Georgia Tech

Dr. William Underwood is a Principal Research Scientist with the Computer Science and Information Technology Division of the Georgia Tech Research Institute in Atlanta. He earned his PhD in Computer Science from the University of Maryland. His current research interests are in developing formal, theoretical foundations for records management and archival science, experimental investigations of alternative digital preservation strategies, and the application of natural language processing, machine learning and knowledge-based reasoning technologies to the support of automated archival description, Freedom of Information Act (FOIA) review, and search and retrieval of records in digital archives. Dr. Underwood’s research, sponsored by the National Archives and Records Administration (NARA), has involved prototyping of an archival repository and archival processing system for accession, arrangement, preservation, review, description and retrieval of electronic records. His current research, sponsored by the National Center for Advanced System technologies (NCAST), seeks to develop tools for information and content extraction from textual documents, induction of grammars for recognizing document types, automatic description of the content of record series, reliable identification of file formats, and decision support for review of Presidential records for Presidential Record Act restrictions and FOIA exemptions. His current research interests are in developing formal, theoretical foundations for records management and archival science, experimental investigations of alternative preservation strategies, and the application of natural language processing technologies to the support of archival description and Freedom of Information Act (FOIA) review.

Over the last dozen years, he has developed forensic (and archival processing) tools for (1) reliably filtering user created files from the contents of hard drives that include operating system and office application software as well, (2) reliably identifying file format types, (currently about 900 file formats), and (3) metadata extraction for hundreds of file formats. In addition, he has contributed more than 100 internal signatures to the PRONOM file format registry for use by the DROID format identification utility.

Underwood was the Principal Investigator of the PERPOS project sponsored by the U S National Archives and Records Administration. The objective of this project was to aid archivists in Presidential Libraries in preserving, reviewing and describing digital records created on personal computers. He was also a member of the US InterPARES II research project sponsored by the National Historical Publications and Records Commission. The objective of that project was to identify technologies and methodologies for long-term preservation of authentic electronic objects created during the course of scientific, artistic and government business activities. He was a member of the Consultative Committee for Space Data Systems, Panel 2 that developed standards for archival information interchange.

### Peter Van Garderen, Artefactual Systems

Peter Van Garderen is project manager for the Archivematica and ICA-AtoM open-source software projects. Peter is also the principal of Artefactual Systems, a Vancouver-based company that provides open-source solutions for the international archival community (see http://artefactual.com).

Peter launched Artefactual Systems Inc. in 2001 to provide technology analysis and implementation services to archival organizations, in particular those that want to develop and implement open-source solutions. Since that time Peter has worked with a wide range of clients, providing services that range from writing strategy reports, analyzing system requirements, designing technology architectures, developing software, and managing open-source projects. Peter is a regular conference speaker on the topics of digital preservation and archives technology.

He has worked at the University of British Columbia’s School of Library, Archival and Information Studies as an Adjunct Professor (1999-2004) and as the Project Coordinator for International Research on Permanent Authentic Records in Electronic Systems (InterPARES Project) (1998-2000). Peter began his career in archives technology over 10 years ago as a product manager for Eloquent Systems (1996-97). Peter is a Distinguished Alumnus of the University of British Columbia’s Master of Archival Studies program and a Doctoral Candidate in Archival Science at the University of Amsterdam.
