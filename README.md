# **Critical Points of Configuration Spaces of Hard Spheres**

This is a database that contains the critical configurations of hard spheres on the rhombic dodecahedron, where the number of hard spheres is $n = 1 \ldots 12$. A critical configuration is one where spheres contacts prevent any collective motion that would allow the radius of all spheres to increase linearly with the extent of the motion. Equivalently, a critical configuration is one that has a mechanically-balanced contact graph. The torus is the rhombic dodecahedron of edge length $3/({2\sqrt{6}})$ with opposite faces identified.

## **Security Statement**
Connecting to a Jupyter notebook server running on your local machine can provide many benefits. With these benefits come serious potential risks. By connecting to a local runtime, you are allowing the Colaboratory frontend to execute code in the notebook using the local resources on your machine. This means that the notebook could:

- Invoke arbitrary commands (e.g. "rm -rf /")
- Access the local file system
- Run malicious content on your machine

Before attempting to connect to a local runtime, make sure you trust the authors of the notebook and ensure you understand what code is being executed. For more information on the Jupyter notebook server's security model, consult [Jupyter's documentation](https://jupyter-notebook.readthedocs.io/en/stable/security.html).

## **Usage**
The capabilities of this notebook are contained in two functions, `import_database` and `plot_crit`. These are defined in the `Define necessary functions` cell (double clicking expands the cell if you would like to examine the code). Run this cell first.

The next cell imports the database of critical points for the desired number of spheres, passed as the single argument to `import_database`. Critical point databases are available for $n=2 \ldots 5$. Running this cell displays the (truncated) table, which you can search for particular values of the index or radius by pressing the `Filter` button. The truncated columns contain information about the positions of the spheres and the contacts between the spheres.

The next cell displays the adjacency matrix and sphere configuration of a selected critical point, passed as the second argument to `plot_crit`. The value of this argument must be an integer that appears in the `crit_number` column of the preceeding data table.

For example, to plot the second critical point for five spheres:
- Run the `Define necessary functions` cell (only needs to be done once)
- Change the argument of `import_database` in the next cell to `5` and run the cell 
- Change the second argument of `plot_crit` in the next cell to `2` and run the cell

## **References**
Research into the topology of the configuration space of hard spheres is ongoing, but the references below provide some context for this project.

- Y. Baryshnikov, P. Bubenik, M. Kahle, [Min-type Morse theory for configuration spaces of hard spheres](https://doi.org/10.1093/imrn/rnt012), International Mathematics Research Notices 2014.9 (2014): 2577–2592.


## **Contributors**
The contributors to this project are (by alphabetical order of last name):

- Ozan Ericok (oericok@ucdavis.edu)
- Kashyap Ganesan (kganesan@ucdavis.edu)
- Jeremy Mason (jkmason@ucdavis.edu)

Please contact Jeremy Mason (jkmason@ucdavis.edu) for more information.

## **License**
The functions included in this archive are licenced under the [GNU General
Public License, Version 3](https://www.gnu.org/licenses/gpl-3.0.en.html).

## **Acknowledgements**
This material is based upon work supported by the National Science Foundation under Grant No. 1839370. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.
