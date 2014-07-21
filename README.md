SciSmalltalk is a new Smalltalk project, similar to existing scientific libraries like NumPy, SciPy for Python or SciRuby for Ruby. SciSmalltalk already provide basic functionalities under MIT licence:
- complex and quaternions extensions,
- random number generators,
- fuzzy algorithms,
- LAPACK linear algebra package,
- Didier Besset's numerical methods,
- Ordinary Differentials Equations (ODE) Solver).

##Build statuses
Last stable version : v0.12

  - Pharo **2**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=20,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=20,VERSION=stable,VM=vm/)
  - Pharo **3**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=30,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=30,VERSION=stable,VM=vm/) 
  - Pharo **4**: [![Build Status](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=40,VERSION=stable,VM=vm/badge/icon)](https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/PHARO=40,VERSION=stable,VM=vm/)

:bangbang: Current active development repository is located at **[SmalltalkHub](http://www.smalltalkhub.com/#!/~SergeStinckwich/SciSmalltalk)**

Some documentation (to be cleaned and reorganized) about SciSmalltalk is available on the Wiki here: 
https://github.com/SergeStinckwich/SciSmalltalk/wiki

We have a continous integration job running here: https://ci.inria.fr/pharo-contribution/job/SciSmalltalk/

##How to install SciSmalltalk in Pharo 2.0/3.0/4.0

If you want to install the last stable version (0.12):

```Smalltalk
Gofer new
	url: 'http://www.smalltalkhub.com/mc/SergeStinckwich/SciSmalltalk/main';
	package: 'ConfigurationOfSciSmalltalk';
	load.
((Smalltalk at: #ConfigurationOfSciSmalltalk) project version: '0.12') load.
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

## How to contribute to SciSmalltalk

We welcome submissions! A google group exists for this project at http://groups.google.com/group/scismalltalk
