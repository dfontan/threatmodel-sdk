[![Build Status](https://travis-ci.org/stevespringett/threatmodel-sdk.svg?branch=master)](https://travis-ci.org/stevespringett/threatmodel-sdk)

ThreatModel SDK
=====================================

The ThreatModel SDK is a minimalistic Java library that provides a basic 
vendor-neutral object model along with the ability to parse reports 
generated from common threat modeling tools.

Supported Threat Modeling Tools
-------------------

* Microsoft Threat Modeling Tool 2016

Planned Threat Modeling Tools
-------------------

* Mozilla SeaSponge

Compiling
-------------------

> $ mvn clean package

Usage Example
-------------------
```java
// Threat model file to open
File file = new File("/path/to/threatmodel.tm7");

// Creates a normalized, vender-neutral ThreatModel object
ThreatModel threatModel = ThreatModelFactory
    .parse(file, ThreatModelingTool.MICROSOFT_THREAT_MODELING_TOOL_2016);
```

Copyright & License
-------------------

ThreatModel SDK is Copyright (c) Steve Springett. All Rights Reserved.

All other trademarks are property of their respective owners.

Permission to modify and redistribute is granted under the terms of the [Apache 2.0] license.

  [Apache 2.0]: http://www.apache.org/licenses/LICENSE-2.0.txt
