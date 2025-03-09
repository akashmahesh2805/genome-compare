# genome-compare
A Rust-based genome comparison visualizer.
# About
genome-compare is a Rust-based tool for visualizing genome alignments and detecting structural variations. The tool parses chain files, identifies structural variations (e.g., inversions, translocations, duplications), and displays the results in an interactive genome browser.
# Features
1. Chain File Parsing
Extracts alignment data from chain files, which describe pairwise alignments between genomes.
Supports standard chain file formats used by UCSC and other genomic databases.

3. Structural Variation Detection
Identifies key structural variations (SVs) relevant to pediatric cancer research:
Inversions: Regions where the genome sequence is flipped.
Translocations: Segments of DNA that have moved to a different chromosome.
Duplications: Repeated regions of the genome.
Deletions: Missing segments of the genome.

3. Interactive Visualization
Displays alignments and structural variations in an intuitive genome browser.
Features:
Blocks or Arcs: Represent aligned regions between two genomes.
Color-Coding: Highlights conservation, divergence, and structural variations.
Zoom and Pan: Allows users to explore specific regions in detail.
Tooltips: Provides detailed information about alignments and SVs.

4. Exportable Visualizations
Saves visualizations as high-resolution images (PNG, SVG) for use in publications or presentations.

# Installation
Clone the repository:
git clone https://github.com/akashmahesh2805/genome-compare.git
cd genome-compare

Build the project:
cargo build --release

Usage:
Visualizing a Chain File
To visualize alignments and structural variations from a chain file:
cargo run -- --chain example.chain

# License
This project is licensed under the Apache License 2.0.
