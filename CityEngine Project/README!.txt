To compile SDK extensions (prt4maya example, stlenc example, custom encoders) it is required to use this 
exact C++ compiler version / boost libraries:
- Microsoft VC10 C++ Compiler (cl.exe) 16.00.40219.01, included in Visual Studio 2010 SP1
- boost 1.53 headers and binaries -> get the boost 1.53 headers from http://www.boost.org
- get the boost 1.53 pre-compiled binaries from http://boost.teeks99.com 
  (e.g. boost_1_53_0-vc64-bin.exe or boost_1_53_0-vc32-bin.exe)
  note: if you compile boost yourself, 
  the boost libraries need to be compiled with correct compiler 
  (VC 10)

In order to COMPILE, you MUST have CityEngine 2013 or later installed on your computer,
you MUST be running at least Windows XP SP1 or later, 
you MUST have either CMake 2.8.10 or later or Visual Studio 2010 (which you will need to compile boost binaries anyway)
- RECOMMENDED: USE VS 2010. Your life will be a lot easier.

Current Known Functionality and Capabilities:
- CityEngine can procedurally generate buildings in areas around streets based on rules.
  <> Rules are written in CGA which is python-like in the way it is written.
  <> It is recommended that you learn python to code CGA as well as if you wish to implement custom
     Export functionality in CE.
  <> Streets can be generated in CE based on pre-obtained Street Data 
     (Check Street Data Tutorial for more info regarding this)

CE's Exported FBX files may be used in either Unity or Unreal Engine. 
However the only PLUGINS available in these respects are the UNITY, MAYA, and CMD plugins
http://lesterbanks.com/2010/01/procedural-shows-off-city-engine-to-unreal-udk/