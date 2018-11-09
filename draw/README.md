# Adding LIMBO bubbles to the LOD cloud
With these scripts you can create diagrams in the style of the openly accessible LOD cloud diagram (https://lod-cloud.net/). The scripts were written by https://github.com/jmccrae. To run the program you need to install Cargo. Once Cargo is installed, in the subfolder /lod-cloud-draw run 

`cargo build --release`

Then copy `data.json`, `output.svg` and `settings.json` from lod-cloud-draw to lod-cloud-draw/target/release and run

`cargo run data.json output.svg -e settings.json`

The files contain the following data

`data.json` - the metadata of datasets in the LOD cloud including the information on the mCloud (https://www.mcloud.de/) metatdata catalog

`output.svg` - an empty .svg file which will contain the LOD diagram after the script has terminated

`settings.json` - the settings for the diagram 

Please note that the script applies a minimization function to determine the optimal parameters for visualization. It either terminates after convergence or 10000 iterations. In case you are generating a diagram for the entire LOD cloud, this may take a couple of hours. 

## Supplementary files
`stat` - folder to store example SPARQL queries that explore statistics from LIMBO datasets

`mcloud-bubble`- metadata catalog of the mcloud, that was added to the public https://lod-cloud.net/lod-data.json to form `data.json`

`limbo.svg` - the visualization of the public LOD cloud plus the LIMBO bubbles (currently only the mCloud metadata catalog

## Up to date source files
This project was taken from the lod-cloud-draw project. In case you want to build this project from up to date sources, please go to https://github.com/lod-cloud/lod-cloud-draw to build you binaries from fresh sources.
