This is the change log of the Refinitiv Real-Time SDK (RTSDK) for Java. RTSDK consists of Enterprise Message API (EMA) and Enterprise Transport API (ETA). This file contains history starting from version 1.2.0 which is when all components (EMA C++, EMA Java, ETA C, ETA Java) of RTSDK were fully open sourced. Note that RTSDK product version numbers start from 1.2.0 and EMA/ETA version numbers start from 3.2.0.

NOTE About Rebranding: Refinitiv Real-Time SDK was formerly known as Elekton SDK or ESDK. Therefore, all versions and fixes prior to RTSDK-1.5.1.L1, may refer to ESDK or Elektron. Fix IDs will continue to refer to ESDK.

There are three types of RTSDK releases that append a letter directly followed by a number to the version number.

"L" releases (e.g., 1.2.0.L1) are full RTSDK releases that are uploaded to MyRefinitiv (formerly Customer Zone), Developer Community and GitHub.
"G" releases (e.g., 1.2.0.G1) are releases that are only uploaded to GitHub.
"E" releases (E-Loads) are emergency RTSDK releases that are uploaded to MyRefinitiv and Developer Community but not to GitHub. Also note that emergency releases may only be partial (i.e., Java or C++/C only).

----------------------------------------------------------------------------------------
CURRENT RELEASE HIGHLIGHTS - RTSDK Java 2.0.0.L1 aka EMA 3.6.0.L1 and ETA 3.6.0.L1
----------------------------------------------------------------------------------------

New Features Added
------------------
The primary object of this release is to completely rebrand RTSDK: change namespace to com.refinitiv, change library names and alter documentation to reflect new branding. A new file explaining impact to customer, REBRAND.md was also added. In addition, there were a few fixes included. This release also introduces qualification on CentOS 8.

Customer Issues Resolved
------------------
- [Case Number: 07508738] - [ESDK-3220] - Using gradlew with example runconsumer113 fails

----------------------------------------------------------------------------------------
FULL CHANGELOG
----------------------------------------------------------------------------------------

--------------------------------------------
RTSDK Java Release 2.0.0.L1 (Oct 19, 2020)
--------------------------------------------

New Features Added
------------------
The primary object of this release is to complete rebranding of RTSDK: change namespace to com.refinitiv, change library names and alter documentation to reflect new branding. A new file explaining impact to customer, REBRAND.md was also added. In addition, there were a few fixes included.

EMA Java 3.6.0.L1 Issues Resolved
---------------------------------
- [ESDK-473] - Incorrect reference to a doc in the Perf Example ReadMe
- [ESDK-3825] - EMAJava - Multiple config files shipped with EmaCpp
- [ESDK-4311] - Application commandline usage/ readme / PDF should NOT make keyfile a mandatory parameter.

ETA Java 3.6.0.L1 Issues Resolved
---------------------------------
- [ESDK-58] - Create training guide for ETA Java
- [ESDK-3220] - Using gradlew with example runconsumer113 fails - [Case Number: 07508738]
- [ESDK-4245] - Change references to UPA or "Ultra Performance API"
- [ESDK-4282] - Received is mis-spelled

Both ETA Java and EMA Java 3.6.0.L1 Issues Resolved
---------------------------------------------------
- [ESDK-3220] - Using gradlew with example runconsumer113 fails - [Case Number: 07508738]
- [ESDK-4151] - Change namespace to refinitiv
- [ESDK-4243] - Documentation: change code snippets to new namespace in all documentation (PDF)
- [ESDK-4244] - Documentation: change namespace references and references to previous product names
- [ESDK-4266] - Documentation: change references to prior product names in code comments 
- [ESDK-4274] - Replace dependent libraries to re-branded for DACS (updated versin of DACS also)
- [ESDK-4283] - Maven Central: register for new namespace
- [ESDK-4285] - Change QA tools to adapt to changes to filenames
- [ESDK-4288] - Create REBRAND.md with customer impacts and add any changes to product names
- [ESDK-4395] - Rebrand: Differentiate between RTSDK product and ETA/EMA library versions

--------------------------------------------
RTSDK Java Release 1.5.1.L1 (Sept 4, 2020)
--------------------------------------------

New Features Added
------------------
This is a maintenance release which resolves customer issus, bugs and adds support for the following: ability to measure tunnel stream performance. Included in this release are rebranding changes.

EMA Java 3.5.1.L1 Issues Resolved
---------------------------------
- [ESDK-475] - EMAJ value add fails to decode message using the DirectoryMsg.decode() method
- [ESDK-1558] - EMAJ: ema.access.DateTimeStringFormatImpl Observation [GitHub #57]
- [ESDK-1633] - Allow EmaConfig.xml to be loaded from jar's resource [GitHub #69, GitHub #126]
- [ESDK-3205] - RDP examples have no text error says could not open keystore file when identify wrong path/file.
- [ESDK-3831] - IndexOutOfBoundsException when trying to access Cloned RefreshMsg EMA Java 1.4 [GitHub #128]
- [ESDK-3835] - EMA ADS connection recovery failure [Case Number: 08431393]
- [ESDK-4092] - EMAJ must check both DictionaryUsed and DictionaryProvided to download dictionary from network
- [ESDK-4178] - Cloning issue with update message when name is included [Case Number: 09046247]

ETA Java 3.5.1.L1 Issues Resolved
---------------------------------
- [ESDK-5] - [Training Examples] Request is for all Training examples to close all open streams and clean up connection upon runtime expiration
- [ESDK-152] - [ Java Training Examples, Cosmetic text changes request ] Consumers show some unnecessary and inconsistent (with C-Edition) text
- [ESDK-307] - ETAJ value add fails to decode message using the DirectoryMsg.decode() method
- [ESDK-310] - No command line in training javadoc
- [ESDK-767] - Example and Training code print statements contain mis-spelling of the word "Received"
- [ESDK-2553] - recvWindowSize (from ETA Java ValueAdd TunnelStream ClassOfService) default value doesn't work as described in the document [Case Number: 07012810]
- [ESDK-3270] - Enhance the Reactor for applications to specify the password for OAuth via the callback method
- [ESDK-3310] - Provides centralize location to keep the OAuth tokens to share between multiple connections using the same OAuth credential
- [ESDK-3473] - ReactorChannel event (Unknown channel event type -3) causing reactor to shutdown
- [ESDK-3773] - Enhance ETAJ Performance tools to support Tunnelstreams
- [ESDK-3865] - ETAJ Client Side Encryption: Add in host name validation, limit TLS version to 1.2, and enable SNI matching in ETAJ
- [ESDK-4083] - Reactor prematurely enters CHANNEL_READY on reconnect [Case Number: 08873087]

Both ETA Java and EMA Java 3.5.1.L1 Issues Resolved
---------------------------------------------------
- [ESDK-3646] - VS2019 Support for JNI
- [ESDK-3672] - Add DACSLock code snippet for ETA/EMA Java into documentation
- [ESDK-3811] - Inefficient java package metadata extract by loop over Package.getPackages() [GitHub #130]
- [ESDK-3828] - Integrate rsslReactorQueryServiceDiscovery() method with centralized token management to reuse token when using same credentials
- [ESDK-3866] - ESDKJ Client Side Encryption: Set default Certificate Authority keystore location in Java so a jks file isn't required
- [ESDK-3867] - ESDKJ Client Side Encryption: Split out encryption and HTTP(S) functionality
- [ESDK-3991] - Provide the ability to configure the takeExclusiveSignOnControl parameter for the password grant type
- [ESDK-4070] - Support a configurable debug parameters to show REST interactions (that do not print credentials)
- [ESDK-4082] - Add tokenScope as a configuration for RDP connectivity
- [ESDK-4090] - Rebranding: Change code references to new product and company name in unit tests, examples, etc.
- [ESDK-4165] - Rebranding: Change references in READMEs, Code Comments,

--------------------------------------------
ESDK Java Release 1.5.0.G1 (Jun 30, 2020)
--------------------------------------------

New Features Added
------------------
This is a maintenance GitHub push which resolves customer issus, bugs and adds support for the following: ability for providers to get round trip latency measurements, provider support for posting, and, openJDK 1.11.

EMA Java 3.5.0.G1 Issues Resolved
---------------------------------
- [ESDK-3844] Network outage related race condition between oauth2 token renewal and login to infra [Case Number: 08453636]
- [ESDK-3854] Support Posting in EMAJ Providers [GitHub #117]
- [ESDK-3883] Documentation correction to specify that SysSendBufSize is applied as number of bytes, not KB [GitHub #137]
- [ESDK-3909] EMA Java indexOutOfBoundsException [Case Number: 08600487]
- [ESDK-3948] Support Round Trip Latency Monitoring
- [ESDK-3988] Change EMA RDP example to take RIC as an input

ETA Java 3.5.0.G1 Issues Resolved
---------------------------------
- [ESDK-773] ETAJ Training Provider Module 5 fails to connect to infra
- [ESDK-1650] rsslDoubleToReal conversion  function doesn't work as expected [Case Number: 06708565]
- [ESDK-3618] Dictionary.entry(int fieldId) returns the same DictionaryEntry instance [Case Number: 07697024 and GitHub # 141]
- [ESDK-3823] Support release of memory used by reactor events by adding maxEventsInPool
- [ESDK-3847] ETA Build warnings using JDK1.11
- [ESDK-3918] ETAJ+Reactor: Suppport Round Trip Latency Monitoring

Both ETA Java and EMA Java 3.5.0.G1 Issues Resolved
---------------------------------------------------
- [ESDK-3696] OpenJDK 1.11 qualification
- [ESDK-4084] EMA should not set compression threshold unless explicitly configured by application 

--------------------------------------------
ESDK Java Release 1.5.0.L1 (Mar 31, 2020)
--------------------------------------------

EMA Java 3.5.0.L1 Issues Resolved
---------------------------------
- [ESDK-3614] EMAJ 'OmmInvalidUsageException', Text='The Field name STOCK_TYPE does not exist in the field dictionary' [Case Number: 07645599]
- [ESDK-3615] Add port info into OmmConsumerEvent::getChannelInformation [GitHub # 113]
- [ESDK-3677] Update the example in the EMA Java config guide to set a default for NumInputBuffers

ETA Java 3.5.0.L1 Issues Resolved
---------------------------------
- [ESDK-45] Watchlist example issue: With service down, posting is still attempted

Both ETA Java and EMA Java 3.5.0.L1 Issues Resolved
---------------------------------------------------
- [ESDK-3834] Update default token service URL to use verison v1

--------------------------------------------
ESDK Java Release 1.4.0.G1 (Jan 10, 2020)
--------------------------------------------

EMA Java 3.4.0.G1 Issues Resolved
---------------------------------
- [ESDK-3472] Added support for NoWait dispatch timeout in Consumer and NiProvider [GitHub # 110] 

Both ETA Java and EMA Java 3.4.0.L1 Issues Resolved
---------------------------------------------------
- [ESDK-3594] Documentation changes with addtional rebranding changes

--------------------------------------------
ESDK Java Release 1.4.0.L1 (Nov 15, 2019)
--------------------------------------------

EMA Java 3.4.0.L1 Issues Resolved
---------------------------------
- [ESDK-3294] Enhancement Request: Added ability to dynamically increase number of allocated output buffers for handling "out of buffers" error [Case Number: 07652023]
- [ESDK-3535] Inconsistency contents in default and description of ReissueTokenAttemptInterval and ReissueTokenAttemptLimit parameter [GitHub #120]

ETA Java 3.4.0.L1 Issues Resolved
---------------------------------
- [ESDK-3204] ESDK Documentation: Fix copyright link after removal of classic portal from esdk repository
- [ESDK-3504] Add option for maxOutputBuffer on ProvPerf
- [ESDK-3506] ETAJ VAConsumer with enable sessionMgnt fails to failover to backup connection on different location

Both ETA Java and EMA Java 3.4.0.L1 Issues Resolved
---------------------------------------------------
- [ESDK-3340] Rebrand ESDK documentation
- [ESDK-3476] Upgrade httpcomponents-core dependency [GitHub # 114]
- [ESDK-3500] Enhancement Request: Add ability to retrieve number of tunnel stream buffers in use

--------------------------------------------
ESDK Java Release 1.3.1.G2 (Oct 18, 2019)
--------------------------------------------

N/A; Changes are limited to ESDK C/C++ ONLY

--------------------------------------------
ESDK Java Release 1.3.1.G1 (Sept 25, 2019)
--------------------------------------------

EMA Java 3.3.1.G1 Issues Resolved
---------------------------------
- [ESDK-3440] Provider fails to accept client connections with dispatch timeOut=NoWaitEnum [GitHub #110] 

ETA Java 3.3.1.G1 Issues Resolved
---------------------------------
- [ESDK-3488] WlLoginHandler does not clear the state of login request for RDP connection
- [ESDK-3423] ETAJ fails to renew token when user specifies non-default token service URL

Both ETA Java and EMA Java 3.3.1.G1 Issues Resolved
---------------------------------------------------
- [ESDK-3430] Add error messages when RDP token request/renewal fails  
- [ESDK-3431] Add TokenReissueRatio, ReissueTokenAttemptLimit and ReissueTokenAttemptLimit into ESDK Java 
- [ESDK-3433] Support configuring RestRequestTimeOut, ReissueTokenAttemptLimit, ReissueTokenAttemptInterval, TokenReissueRatio 
- [ESDK-3468] Add RDP Auth proactive token renewal with password grant prior to refresh token expiration

--------------------------------------------
ESDK Java Release 1.3.1.L1 (July 31, 2019)
--------------------------------------------

New Features Added
------------------
This release adds ability in EMA to clone and copy messages in order to decode payload outside of message callbacks. Please note that client_id is now a manadatory input for Cloud connectivity. ESDK Java now supports JDK 1.11 and OpenJDK 1.8 with an upgrade in gradle version to 5.X. ESDK Java no longer supports JDK1.7.

EMA Java 3.3.1.L1 Issues Resolved
---------------------------------
- [ESDK-1750] Clone/copy facility for message payload to decode it outside of onUpdateMsg() [Case Number: 06854285, 5201994]

ETA Java 3.3.1.L1 Issues Resolved
---------------------------------
- [ESDK-509] Add InitializationTimeout to EMA Config at Channel Level
- [ESDK-900] Change documentation to reflect user-defined Config filename
- [ESDK-1332] Update Consumer340 to increment postId
- [ESDK-2625] Remove Mockito compile dependency from ETAJ [GitHub #94]
- [ESDK-3182] Documentation, ETAJ Dev Guide: Fix "UPA" in Figure 36 to "Transport API Consumer App"
- [ESDK-3183] ETAJ RDP should not perform service discovery lookup when address and port is set by user
- [ESDK-3202] ESDK Documentation: Remove links to "Transport API Value Added Components" in html and refer to VARefman
- [ESDK-3268] Expose ping stats and rsslReadEx in reactor
- [ESDK-3338] Require clientId parameter in ETAJ Reactor

Both ETA Java and EMA Java 3.3.1.L1 Issues Resolved
---------------------------------------------------
- [ESDK-2631] Support JDK 1.11 & Upgrade to Gradle version 5.4.1
- [ESDK-2651] Support OpenJDK 1.8
- [ESDK-3248] With new gradle version, 5.4.1, update documentation to include the -PcommandLineArgs with --args
- [ESDK-3321] Update httpclient and other ESDK jars from 4.X.X to recent version
- [ESDK-3410] Removed extra "/" to service discovery URL to get an Elektron cloud endpoint

--------------------------------------------
ESDK Java Release 1.3.0.G1 (April 16, 2019)
--------------------------------------------

EMA Java 3.3.0.G1 Issues Resolved
---------------------------------
- [ESDK-3194] Documentation improvements for RDP examples [GitHub #98]

ETA Java 3.3.0.L1 Issues Resolved
---------------------------------
- [ESDK-3198] Unsolicited Refresh is not fanned out to first stream when two streams are aggregated by Reactor Watchlist when second stream is a full view. 
- [ESDK-3196] Fix to Watchlist consumer for -tunnel 

--------------------------------------------
ESDK Java Release 1.3.0.L1 (March 26, 2019)
--------------------------------------------

New Features Added
------------------
This ESDK release provides support for RDP Session management (token renewal) and Service Discovery (discovering host/port information based on Cloud region and type of connection ). 

EMA Java 3.3.0.L1 Issues Resolved
---------------------------------
- [ESDK-484] EMA Consumer application that requests a streaming source directory does not receive source directory updates. [Case Number: 05257390]
- [ESDK-619] RMTES Partial updates are not processed correctly if OmmRmtes.toString() is called before OmmRmtes.apply() is called [Case Number: 05533464] 
- [ESDK-1713] Provides interface design and implementation for EMAJ to support session managment from the Reactor
- [ESDK-1766] EMA returns messages to incorrect appClient when OmmConsumer is shared between multiple threads [Case Number: 06902288]
- [ESDK-2597] EMA Consumer application running in User_Dispatch mode sometimes hangs when the upstream source disconnects 
- [ESDK-2599] Require a new utility or interface similar to asHexString that shows raw hex output [Case Number: 07023993]
- [ESDK-2609] Support JDK1.9
- [ESDK-2633] EMA batch requests consume way more memory than the individual requests. [Case Number: 07244571]
- [ESDK-2652] EMAJ Lack of item recovery if service was brought up after consumer was up
- [ESDK-2678] Expose initializationTimeout configuration and make default to higher value for Encrypted

ETA Java 3.3.0.L1 Issues Resolved
---------------------------------
- [ESDK-627] Remove references to UPA in ETA C and ETA Java Developers Guide [Case Number: 05543578]
- [ESDK-1709] Provides HTTP requests for blocking and non-blocking call for ETAJ
- [ESDK-1715] Implements RDP service discovery and token management for ETAJ reactor
- [ESDK-2609] Support JDK1.9
- [ESDK-2624] DateTime is incorrectly implemented as local time rather than GMT [Case Number: 07232265]

--------------------------------------------
ESDK Java Release 1.2.2.L1 (November 15, 2018)
--------------------------------------------

New Features Added
------------------
Provides the functionality for Non-interactive, Interactive, and Consumer applications to get channel information from the EMA's callback methods via OmmProviderEvent and OmmConsumerEvent classes

EMA Java 3.2.2.L1 Issues Resolved
---------------------------------
- [ESDK-800] EMA returns info of all services instead of the requested service [Case Number: 06453247]
- [ESDK-1125] EMA ConsPerf applications do not use specified username in Login Request [Case Number: 05958811]
- [ESDK-1601] Provide channel information in EMA's callback methods [Case Number: 06611113]
- [ESDK-1723] IProvider application with UserDispatch has 100% cpu 
- [ESDK-1724] Fixed a concurrent modification exception in ETAJ Reactor service handling after a disconnect. [GitHub #76] 
- [ESDK-1753] Add support for WindowsServer2016 
- [ESDK-2528] Fix headings syntax in readme [GitHub Pull Request #89]
- [ESDK-2555] Include latest jdacsUpalib.jar in ESDK [Case Number:  06042800 and 06041830]

ETA Java 3.2.2.L1 Issues Resolved
---------------------------------
- [ESDK-647] EMAJ or ETAJ consumer sends duplicate FIDs in a snapshot view request
- [ESDK-1651] UPAJConsPerf throws IllegalArgumentException while connecting when numerous threads attempt to initialize the channel at the same time
- [ESDK-1745] File Descriptor leak open a SocketChannel but never closed [GitHub #78]
- [ESDK-1753] Add support for WindowsServer2016 
- [ESDK-2550] ETA RDM Usage guide section 6.2.4 shows market price update instead of status
- [ESDK-2555] Include latest jdacsUpalib.jar in ESDK [Case Number:  06042800 and 06041830]

--------------------------------------------
ESDK Java Release 1.2.1.L1 (August 15, 2018)
--------------------------------------------

New Features Added
------------------
Programmatic configuration for EMA Consumer, IProvider and NIProvider.

EMA Java 3.2.1.L1 Issues Resolved
---------------------------------
- [ESDK-380] If CompressionType is set to "None", the CompressionThreshold range check still occurs
- [ESDK-415] Clarify parent handle usage in EMA interface [Case Number: 05109877]
- [ESDK-677] Improve reference manual documentation for OmmArray.fixedwidth [Case Number: 05630733]
- [ESDK-705] Programmatic configuration for EMA Java [Case Number: 06558057]
- [ESDK-1513] Eliminate ESDK Java Warnings
- [ESDK-1548] Update RDMUsageGuide to include information on the required filters to mark a service back Up [Case Number: 06538048]
- [ESDK-1587] Deprecate unused StatusCodes [GitHub #65]
- [ESDK-1556] Update JavaDoc for OmmDateTime, OmmDate and OmmTime [GitHub #55]
- [ESDK-1590] Gradlew Build Failed for Elektron SDK Java 1.2.0 package downloaded from the Developer Portal [Case Number: 06591880]
- [ESDK-1596] Data from two different services are mixed up when an item is requested from different services using the same OmmConsumer [Case Number: 06604413]
- [ESDK-1602] Fix EMA/ETA Java Gradle warnings
- [ESDK-1603] toString on a newly created ElementList throws NullPointerException [Case Number: 06589180]
- [ESDK-1640, ESDK-1646] Handle leak in OmmBaseImpl that results in issues while reconnecting [Case Number: 06669026 and GitHub #72]
- [ESDK-1644] Fix README content Github to have change log (without duplicating information)

ETA Java 3.2.1.L1 Issues Resolved
---------------------------------
- [ESDK-380] If CompressionType is set to "None", the CompressionThreshold range check still occurs
- [ESDK-1513] Eliminate ESDK Java Warnings
- [ESDK-1590] Gradlew Build Failed for Elektron SDK Java 1.2.0 package downloaded from the Developer Portal [Case Number: 06591880]
- [ESDK-1602] Fix EMA/ETA Java Gradle warnings
- [ESDK-1635] ETA should not have EDF/Queue examples
- [ESDK-1636] Consumer Module_2_Login training example does not properly fall through
- [ESDK-1644] Fix README content Github to have change log (without duplicating information)

-----------------------------------------
ESDK Java Release 1.2.0.G1 (May 31, 2018)
-----------------------------------------

EMA Java 3.2.0.G1 Issues Resolved
---------------------------------
- [ESDK-1309] EMA Java does not receive NAK when Posting timeout occurs [Case Number: 06037235]
- [ESDK-1446] EMA Java examples missing RMTES data type decoding in decode() function [Case Number: 06453670]
- [ESDK-1481, ESDK-1538] EMA hangs when uninitializing the OmmConsumer [Case Numbers: 06469347, 06466793]
- [[ESDK-1543] Gradle build script must not rely on working dir [GitHub #52]
- [ESDK-1488] EMA Java does not decode the Buffer in a MapEntry key correctly [Case Number: 06486004]

ETA Java 3.2.0.G1 Issues Resolved
---------------------------------
- [ESDK-1415] Incorrect usage of NaN in RealImpl.java [GitHub #51]
- [ESDK-1543] Gradle build script must not rely on working dir [GitHub #52]
- [ESDK-1545] Patterns created for each instance rather than once [GitHub Pull Request #53]

-------------------------------------------
ESDK Java Release 1.2.0.L1 (April 27, 2018)
-------------------------------------------

New Features Added
------------------
ESDK Java now utilizes a Gradle build environment. Refer to the ESDK Java Migration Guide for detailed instructions regarding how to build EMA Java with Gradle.

EMA now supports encrypted connection type.

EMA Java 3.2.0.L1 Issues Resolved
---------------------------------
- [ESDK-487] EMA throws OmmInvalidUsageException if an empty Map is encoded [Case Number: 05338640 and GitHub #28]
- [ESDK-907] EMA can't handle a SERVICE_DIRECTORY refresh that contains a lot of services [Case Number: 05896732, 06042281 and 06443659]
- [ESDK-929] EMA Java application does not receive updates after received the Status Message with no State information [Case  Number: 06436262 and GitHub #37]
- [ESDK-943] Update EMAJ OmmBuffer documentation
- [ESDK-417] Expose encrypted connection support through EMA Java
- [ESDK-813] Date/Time/DateTime to string and from string conversions should support ISO 8601 format.
- [ESDK-1120] ConcurrentModificationException in EMA [GitHub #34]
- [ESDK-1218] EMA application uses 100% CPU and hangs when it makes a lot of requests and the monitor shows a large number of instances of WorkerEvent [Case  Number: 06393015 and GitHub #41]
- [ESDK-1220] ConcurrentModificationException while invoking dispatch() [Case Number: 06107164]
- [ESDK-1307] ETAJ connected component could not set for HTTP and HTTPS type connections
- [ESDK-1360] EMA Java Tunnel Stream sub-stream with stream id gets NullPointerException
- [ESDK-1364] AckMsgImpl toString() method typo
- [ESDK-1365] ItemCallbackClient NullPointerException when rsslMsg state is null
- [ESDK-1388] Mavenize the build [GitHub #21]
- [ESDK-1431] EMA Java cannot handle negative FIDs in View request [Case Number: 06444345]

ETA Java 3.2.0.L1 Issues Resolved
---------------------------------
- [ESDK-676] EMA Java batch consumer encounters "Reactor is shutdown, submit aborted" error status [Case Number: 05633341]
- [ESDK-907] EMA can't handle a SERVICE_DIRECTORY refresh that contains a lot of services [Case Number: 05896732, 06042281 and 06443659]
- [ESDK-929] EMA Java application does not receive updates after received the Status Message with no State information [Case Number: 06436262 and GitHub #37]
- [ESDK-1062] EMA Java encountered java.lang.NullPointerException [Case Number: 06107469 and 05958461]
- [ESDK-1064] Exception when set http with proxy using Consumer
- [ESDK-1218] EMA application uses 100% CPU and hangs when it makes a lot of requests and the monitor shows a large number of instances of WorkerEvent [Case Number: 06393015 and GitHub #41]
- [ESDK-1227] Exception reactor.ReactorChannel.releaseBuffer(ReactorChannel.java:658)
- [ESDK-1300] Review/refactor ETAJ Watchlist Recovery & Cleanup Code
- [ESDK-1385] Watchlist consumer returns a ‘NullPointerException” when same item is used with private, private view & snapshot
- [ESDK-1388] Mavenize the build [GitHub #21]
- [ESDK-1489] ETA Java adds payload when container type is set to NO_DATA [Case Number: 06475782]
