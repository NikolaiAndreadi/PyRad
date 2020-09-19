# PyRad
This script package was developed for the creation and analysis of radiolysis systems.

The main software to do all TDDFT calculations: qb@ll (https://github.com/LLNL/qball)
You will also need the packmol software to create systems (http://m3g.iqm.unicamp.br/packmol/home.shtml)

This repo includes:

1) PyRadCreator - creates enviroment for radyolysis calculation in qb@ll software.
Usage: PyRadCreator.py input1.ini input2.ini
.ini files, and the host .xyz files should be placed in the same directory as this script.
all pseudopotentials should be placed in pseudos directory

2) PyRadTester - H2O radicals searcher with simple gui.
Usage: PyRadTester.py qball_out.o

3) PyRadEDensity - analyses electron density .cube file and findes all anomalies in it. With simple gui.
Usage: PyRadTester.py cube_file.o
on GUI: symbols - atoms
        colored dots - electron density maxima
        sample size and threshold - sliders for maxima searcher
        correlation - slider to filter out electron density maxima that appear near atoms
