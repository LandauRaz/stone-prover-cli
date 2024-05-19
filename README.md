# Stone Prover CLI

A simple interface for using the Stone prover.

## Install

For now, only Linux platforms are supported.

### Installing dependencies

```shell
sudo apt install libdw1 wget
```

### Installing the CLI

```shell
wget -O - https://raw.githubusercontent.com/Moonsong-Labs/stone-prover-cli/main/scripts/install-stone-cli.sh | bash
```

## Usage

### Proving Cairo PIEs

After generating one or more Cairo PIEs (see [cairo-vm](https://github.com/lambdaclass/cairo-vm/tree/main) for more details), run:

```shell
stone-prover-cli prove pie1.zip pie2.zip ...
```

### Verify a proof

To verify the generated proof file, run:

```shell
stone-prover-cli verify proof.json
```