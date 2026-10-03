# sgp4-cpp

Vallado's SGP4 C++ implementation, preserved as used by
[ASTROCHRON](https://github.com/KaffuAlcaid/ASTROCHRON).

## Source

- Upstream: [brandon-rhodes/python-sgp4](https://github.com/brandon-rhodes/python-sgp4)
- Upstream commit: `bf25b00ccf8cf0770a8e5ba458134156f1c70812`
- Original files: `extension/SGP4.cpp`, `extension/SGP4.h`, and `LICENSE`
- Source snapshot: [upstream tree](https://github.com/brandon-rhodes/python-sgp4/tree/bf25b00ccf8cf0770a8e5ba458134156f1c70812)

The source header identifies the implementation as `SGP4 Version 2020-07-13`.
This repository contains the C++ implementation without the Python bindings.

## Local Differences

Compared with the recorded upstream commit, this copy retains ASTROCHRON's
five adjustments to `sscanf_s` calls under MSVC: buffer-size arguments use
unsigned integer literals (`6u`, `1u`, and `11u`) instead of expressions
involving `sizeof(char)`. The remaining differences are whitespace and
line-ending normalization. The orbital propagation equations are unchanged.

## License

The upstream MIT license and copyright notice are preserved in [LICENSE](LICENSE).
