# DNA Data Encoding

This repository contains code for encoding, storing, and decoding digital data in DNA strands.

## Overview

DNA data storage takes advantage of DNA's ultra-high storage density and durability to archive data for decades or centuries. This repository implements an end-to-end workflow for encoding data into DNA, synthesizing and retrieving the DNA strands, and decoding the data back into its original digital form.

Key capabilities demonstrated:

- Encoding text, image, audio, and video files into DNA base sequences 
- Synthetic DNA synthesis and sequencing integration
- Random access of subsets of encoded data
- Data recovery via PCR amplification and nanopore sequencing
- Encryption for data security

## Getting Started

The encoder and decoder modules require Python 3.6 or higher. Key dependencies include:

- biopython
- dnaio
- pandas 
- matplotlib
- numpy

To install:

```
pip install -r requirements.txt
```

Encode sample data:

```
python encode.py sample_data/ sample_encoded.dnadata
``` 

Decode DNA data:

```
python decode.py sample_encoded.dnadata decoded_data/
```

## Usage Examples

- [Encoding an image](docs/encode_image.md)
- [Reading specific data sections](docs/selective_access.md) 
- [Data recovery from damaged DNA](docs/error_correction.md)

## Contributors

Contributions to improve the encoding schemes, add capabilities, and fix bugs are welcome! Please submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References

Relevant papers on DNA data encoding:

1. Church et al, "Next Generation Digital Information Storage in DNA" 
2. Grass et al, "Robust Chemical Preservation of Digital Information on DNA in Silica with Error-Correcting Codes"
3. Yazdi et al, "A Rewritable, Random-Access DNA-Based Storage System"
