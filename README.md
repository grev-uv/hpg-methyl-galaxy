# hpg-methyl-galaxy

Galaxy plugin of the HPG-Methyl aligner and methylation caller.

## Initial configuration

1. If you want to enable user-generated genomic indices, also add the `hpgmethyl_index.xml` tool entry.
2. Edit `hpgmethyl.xml` to set-up the paths to the built-in genomic indices. Modify the indicated
   entries in the `<command>` tag.
3. Enable or disable user-generated indices or any of the built-in genomic indices commenting or uncommenting
   the entries in the `input_gen_selector` tag, as specified in the comments of the XML file.
4. Manually generate the built-in indices if they're enabled. Check the documentation of 
   [HPG-Methyl](https://github.com/grev-uv/hpg-methyl) for instructions on how to generate the indices.

**Warning:** Genomic indices can take a large ammount of disk space. For the GRCh37 reference genome, the corresponding
index size is around **237 GB**. Ensure that the target filesystem has enough disk space and users have enough disk quota
before enabling custom genomic index generation.

## Manual installation instructions

In case you don't want to install the tool from the public toolshed, it can be installed manually:

1. Download the latest relase of the plugin from the Releases section.
2. Decompress the `.tar.gz` package to `GALAXY_DIR/tools/`.
3. Add the tool entries for `hpgmethyl.xml` to `GALAXY_DIR/config/tool_config.xml`.

## License and contribution

HPG-Methyl and its Galaxy plugin are free software and licensed under the GNU General Public License version 2. 
Check the COPYING file for more information.

Contact any of the following developers for any enquiry:

* Juanma Orduña ([juan.orduna@uv.es](mailto:juan.orduna@uv.es)).
* Mariano Pérez ([mariano.perez@uv.es](mailto:mariano.perez@uv.es)).
* Ricardo Olanda ([ricardo.olanda@uv.es](mailto:ricardo.olanda@uv.es)).
* César González ([cesar.gonzalez-segura@uv.es](mailto:cesar.gonzalez-segura@uv.es)).
