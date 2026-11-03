# Raw data: ALS beamtime 20260423

**Logbook entry: <https://diffuse.science/logbook/beamtime/20260423_als/>**

This repository catalogs the raw data from one beamtime of [The Diffuse Project](https://prismscience.org/science/accelerating-dynamic-data-collection#diffuse-scattering) at beamline 8.3.1 of the Advanced Light Source (ALS). The logbook entry above describes the samples, the experiments, and the data processing results. Entries for all beamtimes are in the [logbook](https://diffuse.science/logbook/beamtime).

It is a [DataLad](https://www.datalad.org) dataset. Git holds the directory tree and file checksums. The file contents are tracked with [git-annex](https://git-annex.branchable.com) and hosted on the [Open Storage Network](https://www.openstoragenetwork.org) (OSN), at `https://nyu1.osn.mghpcc.org/diffuse-als-public/20260423/`. Anyone can download the files without an account, and every download is checked against its recorded checksum. Data on OSN are not modified after they are written.

## Usage

Install DataLad, which requires git-annex (for example, `mamba install -c conda-forge datalad`). Cloning downloads only file names and metadata. File contents are fetched on request.

```bash
datalad clone https://github.com/prism-science/diffuse-data-raw-als-20260423.git
cd diffuse-data-raw-als-20260423

# fetch one file or directory
datalad get <path>

# fetch everything, four files at a time (diffraction images can be large)
datalad get -J4 .

# free up disk space when finished
datalad drop <path>
```

Plain git and git-annex also work:

```bash
git clone https://github.com/prism-science/diffuse-data-raw-als-20260423.git
cd diffuse-data-raw-als-20260423
git annex init
git annex get <path>
```

To download single files without git, use `https://nyu1.osn.mghpcc.org/diffuse-als-public/20260423/<path>`.

## Acknowledgments

This work was supported by Radial, a division of Astera Institute.

Beamline 8.3.1 at the Advanced Light Source is operated by the University of California San Francisco with generous support from the National Institutes of Health (P30 GM124169 for user support), and the Integrated Diffraction Analysis Technologies program of the US Department of Energy Office of Biological and Environmental Research. The Advanced Light Source (Berkeley, CA) is a national user facility operated by Lawrence Berkeley National Laboratory on behalf of the US Department of Energy under contract number DE-AC02-05CH11231, Office of Basic Energy Sciences.

Raw data are shared publicly on the Open Storage Network (OSN) via project allocation BIO250275 from [ACCESS](https://access-ci.org), supported by U.S. National Science Foundation (NSF) grants #2138259, #2138286, #2138307, #2137603, and #2138296.
