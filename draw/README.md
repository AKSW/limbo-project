
# Adding LIMBO bubbles to the LOD cloud
With these scripts you can create diagrams in the style of the openly accessible LOD cloud diagram (https://lod-cloud.net/). The scripts were written by https://github.com/jmccrae. To run the program you need to install Cargo. Once Cargo is installed, in your project folder navigate to target/release and run

cargo run data.json output.svg -e settings.json

The files data.json, output.svg and settings.json are already provided in the folder. They contain

data.json - the metadata of datasets in the LOD cloud including the information on the mCloud (https://www.mcloud.de/) metatdata catalog
output.svg - an empty .svg file which will contain the LOD diagram after the script has terminated
settings.json - the settings  for the diagram 

# Supplementary files



# Up to date source files
This project was taken from the lod-cloud-draw project. In case you want to build this project from up to date sources, please go to https://github.com/lod-cloud/lod-cloud-draw. Build the project with 

cargo build --release

Add the files <data.json>, <settings.json> and <output.svg> to any subfolder under your source directory, preferably under target/release to access them right away.
