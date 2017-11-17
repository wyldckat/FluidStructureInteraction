Fluid-Structure Interaction - Toolkit
=====================================

Quoting from here: http://www.cfd-online.com/Forums/openfoam-news-announcements-other/106881-solid-mechanics-solvers-added-openfoam-extend.html#post547754

> This toolkit supersedes the `icoFsiElasticNonLinULSolidFoam` FSI solver within the solidMechanics toolbox.

> This framework was presented at the OpenFOAM Workshop 2014 in Zagreb:
>   - abstract: http://sourceforge.net/projects/openfoam-extend/files/OpenFOAM_Workshops/OFW9_2014_Zagreb/Abstracts/Zeljko_Tukovic_OFW09_EA_0103.pdf
>   - slides: http://sourceforge.net/projects/openfoam-extend/files/OpenFOAM_Workshops/OFW9_2014_Zagreb/Presentations/Zeljko_Tukovic_OFW09_P_0103.pdf

> The major improvement with regard to FSI coupling is the implementation of the IQN-ILS algorithm.
> Also, the plugin approach used for the solid and fluid solvers should allow easier extension to other fluid/solid models e.g. multi-phase, compressible, plasticity, etc.

For **more details** about this toolkit, including **how to use** and **install/build it**, check the associated wiki page: http://openfoamwiki.net/index.php/Extend-bazaar/Toolkits/Fluid-structure_interaction


Original Authors
================

 * solidMechanics toolbox: Philip Cardiff, University College Dublin.

 * FluidStructureInteraction toolkit: Zeljko Tukovic, P. Cardiff, A. Karac, H. Jasak, A. Ivankovic

    * For proper punctuation of the names, please see the "slides" document listed above.


Further modifications
=====================

Original source came from the wiki page: http://openfoamwiki.net/index.php/Extend-bazaar/Toolkits/Fluid-structure_interaction

Further modifications made by Bruno Santos (wyldckat@github working at [blueCAPE Lda](http://www.bluecape.com.pt)):

 * Gitified the source code.
 * Adjusted the code for building properly with the more recent foam-extend 3.1 and 3.2
 * Improved building organization for taking full advantage of parallel building.

 
Git branches
============

Currently there are only three branches:

  * [fe30](https://github.com/wyldckat/FluidStructureInteraction/tree/fe30) - This branch will build as-is with foam-extend 3.0
  * [fe31](https://github.com/wyldckat/FluidStructureInteraction/tree/fe31) - This branch will build as-is with foam-extend 3.1
  * [fe32](https://github.com/wyldckat/FluidStructureInteraction/tree/fe32) - This branch will build as-is with foam-extend 3.2

Quick usage instructions:

  1. Clone the repository:
  ```
  git clone https://github.com/wyldckat/FluidStructureInteraction.git
  ```
  
  2. Checkout the right branch, e.g. for `fe30`:
  ```
  cd FluidStructureInteraction
  git checkout fe30
  ```

  3. Now build:
  ```
  cd src
  ./Allwmake
  ```


License
=======

The same as foam-extend, namely GNU GPL v3. For more information, see the file LICENSE or COPYING, depending on the branch on this repository.
