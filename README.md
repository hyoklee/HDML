# Hyper-Data Markup Language

This is a project for augmenting/subsetting/aggregating data freely from multiple data sources such as MS Excel, DB, Hadoop, and other binary formats such as netCDF. The development goal is to make HDML as the DNA of all data - simple, elegant, and universal. 

Here are a few example data sources:

1. src=”hdf4://AIRS.hdf/path/to/dset[0:2:4, 0:3:6]” You can replace hdf4 to hdf5/netcdf/geotiff.
2. src=”excel://myexcel.xls/sheet1/A3:C10”
3. src=”mysql://host:3306/user:password/SQLstatement”
4. src=”hdfs://node:8020/user/hadoop/…”
5. src=”s3://landsat-pds/L8/003/017/LC…” for Amazon S3
6. src=”opendap://acdisc.sci.gsfc.nasa.gov/opendap/ncml/Aqua_AIRS_Level3/AIRH3ST8.005/2002/AIRS.2002.09.01.L3.RetStd_H008.v5.0.14.0.G07183213133.hdf.ncml.ascii?TotalCounts_A[0:100:179][0:100:359]”
