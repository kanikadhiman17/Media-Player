# Media-PlayerTOOLS USED
⦁	    NetBeans IDE to develop the project.
⦁	    Scene Builder to build the Interface.


Platform : 	 			 Java
Programming Language : 	 Java
IDE Tool : 				 Netbeans
Interface Builder:			 Scene Builder
Database : 	 			 No
Project Type : 	 		 Desktop Application

# Introduction
The Media Player is completely an implementation of the interfaces, classes and methods inbuilt in Java Media FrameWork(JMF). Yhe main purpose of this player is to provide a simple and reliable player independent of platforms.

# Functions:
⦁	Play
⦁	Pause
⦁	Rewind
⦁	stop
⦁	Volume Control
⦁	Timeline
⦁	Speed

# Data Model
• JMF media players usually use DataSources to manage the
transfer of media-content. A DataSource encapsulates both
the location of media and the protocol and software used to
deliver the media. Once obtained, the source cannot be reused
to deliver other media.
• A DataSource is identified by either a JMF MediaLocator or
a URL (universal resource locator). A MediaLocator is similar
to a URL and can be constructed from a URL, but can be
constructed even if the corresponding protocol handler is not
installed on the system. (Note: In Java, a URL can only be
constructed if the corresponding protocol handler is installed on
the system.)
– A standard data source uses a byte array as the unit of transfer. A
buffer data source uses a Buffer object as its unit of transfer.
• JMF data sources can be categorized according to how data
transfer is initiated:
– Pull Data-Source--the client initiates the data transfer and controls
the flow of data from pull data-sources.
– Push Data-Source--the server initiates the data transfer and
controls the flow of data from a push data-source. Push datasources include broadcast media, multicast media, and video-ondemand (VOD).

# Managers
• JMF uses four managers:
– Manager--handles the construction of Players,
Processors, DataSources, and DataSinks. This level of
indirection allows new implementations to be
integrated seamlessly with JMF.
– PackageManager--maintains a registry of packages
that contain JMF classes, such as custom Players,
Processors, DataSources, and DataSinks.
– CaptureDeviceManager--maintains a registry of
available capture devices.
– PlugInManager--maintains a registry of available JMF
plug-in processing components, such as Multiplexers,
Demultiplexers, Codecs, Effects, and Renderers.
JMF: Main Functionality
• Presentation
– Take media content from a DataSource and render it.
– This functionality is contained in the Controller interface
• Player extends this interface
• Processing
– Take media content from a DataSource, perform some userdefined processing on it, and output it
– This functionality is contained in the Processor interface
• Processor extends the Player interface
• Capture
– A capturing device can act as a source for multimedia data.
– Capture devices are abstracted as DataSources.
• Media Storage and Transmission
– A DataSink reads media data from a DataSource and renders
it to some destination (generally a destination other than a
presentation device).
– E.g., A DataSink might write data to a file, write data across the
network.

# Player
• A Player processes an input stream of media data and
renders it at a precise time. A DataSource is used to
deliver the input media-stream to the Player.The
rendering destination depends on the type of media being
presented.

# HOW TO RUN THIS PROJECT
⦁	Import the project on the NetBeans IDE and run it
