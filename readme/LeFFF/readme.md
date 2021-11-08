# Original data

The Lexique des Formes Fléchies du Français (LeFFF in the following) is licenced
under the terms given in the LGPL-LR. A `LICENSE` file should be in the same
folder, giving you the full text of the license.

You can download the original data from the following url :
https://gforge.inria.fr/frs/download.php/file/34602/lefff-3.4.elex.tgz

# Modifications to the original resource and how to recreate the data

The original LeFFF was modified to be used in SEM as an external resource for
some of the available pipelines. Wapiti models marked as ".lefff" use LeFFF as
a resource, worflow that use any ".lefff" model uses LeFFF as a resource.

A (now lost) program used to do the following:

- translate categories present in LeFFF into an FTB POS tags, the map itself
(from a LeFFF category to an FTB POS tag) was created by hand.
- create one file per FTB POS tag
- fill each of those files with lexical forms found in LeFFF that fit into each
category.

The result of this program is in the folder
`resource-pack/fr/base.tar.gz/dictionaries/fr/lefff`, every file in this folder
is a direct derived work from LeFFF and is under the same licence as LeFFF.
