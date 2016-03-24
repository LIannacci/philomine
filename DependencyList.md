PhiloMine should run on any OS-X or Linux machine.  The more memory
and faster machine the better.  We have had success using a Mac
G5 Quad Core with 2GB memory and a Mac G5 Dual Quad Core with 12 GB memory.

We are very dependent, in a very good sense, on many fine open source packages.  Here is the list of (mainly) required packages (not all are required for all functions):

Required for all functions:
  * [PhiloLogic3](http://philologic.uchicago.edu/download.php) (available from those good lads at ARTFL)
  * PhiloLogic loader modifications (in this distribution)
  * [MySQL](http://www.google.com/search?client=safari&rls=en&q=mysql&ie=UTF-8&oe=UTF-8)
  * [YAML](http://search.cpan.org/~ingy/YAML-0.62/lib/YAML.pm)

Required Perl Modules:
  * CGI; URI::Escape; POSIX; (probably already available to you)
  * IO::Tee; http://search.cpan.org/~kenshan/IO-Tee-0.64/Tee.pm

Required to generate lemmas:
  * [Alvis::Treetagger](http://search.cpan.org/~wbuntine/Alvis-QueryFilter-0.3/lib/Alvis/Treetagger.pm) (for philomineload) - A special hacked version is needed for each language you wish to use. A French and English version is provided in the perl\_mods directory of the installation tarball. Install Alvis::Treetagger and copy these into the install directory.
  * [Lingua::Stem::Fr](http://search.cpan.org/~sdp/Lingua-Stem-Fr-0.02/lib/Lingua/Stem/Fr.pm)
  * [TreeTagger](http://www.ims.uni-stuttgart.de/projekte/corplex/TreeTagger/) and French English parameter files (for philomineload)


Required for specific mining functions:
  * [Weka3](http://www.cs.waikato.ac.nz/~ml/weka/) (run from command line)
  * [SVMLight](http://svmlight.joachims.org/) (run from command line)
  * [perlmods](http://www.cpan.org/)
  * [Algorithm::NaiveBayes](http://search.cpan.org/dist/Algorithm-NaiveBayes/)
  * [AI::DecisionTree](http://search.cpan.org/dist/AI-DecisionTree/)
  * [GraphViz](http://search.cpan.org/~lbrocard/GraphViz-2.02/lib/GraphViz.pm)
  * [CLUTO](http://glaros.dtc.umn.edu/gkhome/views/cluto)



Let us know if we missed something.

Not all dependencies are required for all classifiers. If you don't want to use SVMLight or Weka functions, for example, they needn't be installed and the other PhiloMine functions will be accessible if they are installed.