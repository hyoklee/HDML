# Hyper-Data Markup Language
HDML is a language for data virtualization. HTML has allowed us to compose texts and images freely and present them through web browser. So, why not for data?

## Easy to Create Dashboard

HDML makes Dashboard creation as easy as publishing an HTML web page.

## Data for Everyone

This is a project for augmenting, subsetting, and aggregating data freely from multiple data sources such as MS Excel, DB, Parquet on Hadoop Distributed File System (HDFS) or AWS S3, and other binary formats such as netCDF. The development goal is to make HDML as the DNA of all data - simple, elegant, and universal. 

HTML5 provides data tag. HDML expands it with src attribute.  

Here are a few example data sources:

1. src=”hdf4://AIRS.hdf/path/to/dset[0:2:4, 0:3:6]” You can replace hdf4 to hdf5/netcdf/geotiff.
2. src=”excel://myexcel.xls/sheet1/A3:C10”
3. src=”mysql://host:3306/user:password/SQLstatement”
4. src=”hdfs://node:8020/user/hadoop/…”
5. src=”s3://landsat-pds/L8/003/017/LC…” for Amazon S3
6. src=”opendap://acdisc.sci.gsfc.nasa.gov/opendap/ncml/Aqua_AIRS_Level3/AIRH3ST8.005/2002/AIRS.2002.09.01.L3.RetStd_H008.v5.0.14.0.G07183213133.hdf.ncml.ascii?TotalCounts_A[0][3]”
7. src="random" (Fill with random values)
8. src="_FillValue" (Fill data with fill value)
9. src="increasing" or "decreasing" (Fill data with monotonically increasing values that datatype allows. Repeat when overflow occurs)
10. src="ipfs://..."?

