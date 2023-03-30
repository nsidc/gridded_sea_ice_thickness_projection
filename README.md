<p align="center">
  <img alt="NSIDC logo" src="https://nsidc.org/themes/custom/nsidc/logo.svg" width="150" />
</p>


# Gridded Observational Sea Ice Thickness Projection and Grid

Gridded Observational Sea Ice Thickness Projection and Grid describes is _the hidden manual_ for how to add projection and grid information the netCDF files in [NSIDC-0690](https://nsidc.org/data/nsidc-0690/versions/1).

Gridded Observational Sea Ice Thickness Products are grids of long-term mean spring ice thickness derived from ERS-1 (1993-2001) and CryoSat (2011 to 2013) radar altimeters, ICESat laser altimeter (2004 to 2009), Operation IceBridge airborne altimeter and snow radar (2009 to 2014), and submarine upward looking sonar (1986-).  These data have been resampled and gridded to a common EASE Grid with 100 km cell size.  All satellite-derived ice thickness fields were regridded as needed from their original gridded format to 100-km EASE grids using a drop-in-the-bucket averaging. IceBridge and submarine thickness estimates within 70 km of a 100 km EASE grid box center were averaged to give a grid cell mean thickness.  Data are written to netCDF files.

Unfortunately, the files have sparse metadata and do not provide projection or grid coordinate information, and they do not conform to the netCDF CF-Convention standard.  The notebook and other information in this repo aims to remedy this situation.


## Level of Support

* This repository is not actively supported by NSIDC but we welcome issue submissions and
  pull requests in order to foster community contribution.

See the [LICENSE](LICENSE) for details on permissions and warranties. Please contact
nsidc@nsidc.org for more information.


## Requirements

- `jupyter lab`  
- `xarray`  
- `pyproj`
- `pytest`

Full dependencies are in `environment.yml`

## Installation

`git clone `

## Usage

```
$ jupyter lab  # or however you start a jupyter lab instance
```

Run the notebook


## Troubleshooting

TBD

## License

See [LICENSE](LICENSE).


## Code of Conduct

See [Code of Conduct](CODE_OF_CONDUCT.md).


## Credit

This content was developed by the National Snow and Ice Data Center with funding from
multiple sources.
