SciSmalltalk is a new Smalltalk project, similar to existing scientific libraries like NumPy, SciPy for Python or SciRuby for Ruby. SciSmalltalk already provide the following basic functionalities:
- complex and quaternions extensions,
- random number generators,
- fuzzy algorithms,
- KDE-trees,
- Didier Besset's numerical methods,
- Ordinary Differential Equation (ODE) solvers.

[![Lorentz attractor with SciSmalltalk and GraphET](https://pbs.twimg.com/media/Ble65B3CYAEkMoR.jpg)](https://twitter.com/SergeStinckwich/status/457039376111788032)

:bangbang: Current active development repository is located at **[SmalltalkHub](http://www.smalltalkhub.com/#!/~SergeStinckwich/SciSmalltalk)**

Some documentation (to be cleaned and reorganized) about SciSmalltalk is available on the Wiki here: 
https://github.com/SergeStinckwich/SciSmalltalk/wiki

Natalia wrote some explanation about benchmarking SciSmalltalk in the Pharo For Enterprise Book: https://github.com/SquareBracketAssociates/PharoForTheEnterprise-english/blob/ae40e7ab6f7651f6e7c271869eb1efc4e531e774/ComparingSolutions/ComparingSolutions.pier

##Build statuses
Last stable version : v0.13

We have a continous integration job running here: https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/

  - Pharo **2**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=20,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=20,VERSION=stable,VM=vm/)
  - Pharo **3**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=30,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=30,VERSION=stable,VM=vm/) 
  - Pharo **4**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=40,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=40,VERSION=stable,VM=vm/)


##How to install SciSmalltalk in Pharo 2.0/3.0/4.0 and Squeak 4.5

If you want to install the last stable version (0.13):

```Smalltalk
Gofer new
	url: 'http://www.smalltalkhub.com/mc/SergeStinckwich/SciSmalltalk/main';
	package: 'ConfigurationOfSciSmalltalk';
	load.
((Smalltalk at: #ConfigurationOfSciSmalltalk) project version: '0.13') load.
```

If you want to install the development version :

```Smalltalk
Gofer new
	url: 'http://www.smalltalkhub.com/mc/SergeStinckwich/SciSmalltalk/main';
	package: 'ConfigurationOfSciSmalltalk';
	load.
(Smalltalk at: #ConfigurationOfSciSmalltalk) loadDevelopment.
```

All packages load into the Math-* package names.

## Licence
SciSmalltalk is licensed under MIT. See : http://opensource.org/licenses/MIT

## How to contribute to SciSmalltalk

We welcome submissions! A google group exists for this project at http://groups.google.com/group/scismalltalk
