# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

   https://user-images.githubusercontent.com/122033587/279098403-e1cbafff-3772-4eb1-aa74-1cf7de1033d8.png

2.	Install java1.8 in folder /usr/local

    https://user-images.githubusercontent.com/122033587/279098478-3afdd0ff-c77f-40c5-93a2-733a8c354afa.png	
  
3.	Install Hadoop

   https://user-images.githubusercontent.com/122033587/279098529-e4b32179-a598-4ff8-8ca1-0a6a3bdf1040.png

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

https://user-images.githubusercontent.com/122033587/279098607-e6817394-1d64-4834-861b-70db6c0bf2ad.png
 
5.	Set hadoop environment variables: Include the following lines /etc/profile file

	https://user-images.githubusercontent.com/122033587/279098656-5aedd4db-8b1d-4743-aa73-751014006f54.png


6.	Run the.bashrc & profile files from the $ prompt for updating the changes

	  https://user-images.githubusercontent.com/122033587/279098701-3b71c2ea-8d17-4ec8-8f73-8b242dd581c0.png




$ bin/hadoop version	

https://user-images.githubusercontent.com/122033587/279098741-2b4d4fef-a41f-4c93-bd76-ac796a4c7939.png

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

https://user-images.githubusercontent.com/122033587/279098854-a553ecb7-58fc-4e5d-9ff9-0d4f9f27da77.png

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

https://user-images.githubusercontent.com/122033587/279098917-c37367a3-624d-4c74-81e3-c0bf43e309a9.png




 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

https://user-images.githubusercontent.com/122033587/279099714-64a73bd1-d22a-46a2-8caf-2c677f8ba4fd.png

c)	mapred-site.xml
 

Include the following lines in mapred-site.xml file

https://user-images.githubusercontent.com/122033587/279099855-fc84e61f-fd74-4e1e-8a6a-88c8928bbeaf.png

 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

https://user-images.githubusercontent.com/122033587/279100405-46d58e22-8462-4e3e-a588-44022f080462.png


e)	yarn-site.xml
Include the following lines in yarn-site.xml file

https://user-images.githubusercontent.com/122033587/279100622-3ce294b7-f16a-4c06-b9d9-82597a0a9c81.png
8.	Format the Hadoop File system implemented on top of the local file system using

9.	Start Hadoop using


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

https://user-images.githubusercontent.com/122033587/279101477-30e0de2d-964a-485b-9bd6-8a290ff5a391.png

11.	Create a directory ‘/input’ in HDFS

https://user-images.githubusercontent.com/122033587/279101601-68058b0f-f0f9-47bf-a8bf-d487f762f7c6.png

12.	Copy the input files into the distributed file system

https://user-images.githubusercontent.com/122033587/279101755-eddd87cf-12a4-428f-9826-2280fb72408f.png

13.	Run some of the examples provided


14.	Examine the output files
Copy the output files from the distributed file system to the local file system and examine them:
 
or
View the output files on the distributed file system

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
