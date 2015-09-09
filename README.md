# Raspberry Pi image generator

This scripts simplified the process of create a personalized image for the
raspberry pi. They ara based on the work of Petter Reinholdtsen at [Teaching vmdebootstrap to create Raspberry PI SD card images](http://people.skolelinux.org/pere/blog/Teaching_vmdebootstrap_to_create_Raspberry_Pi_SD_card_images.html).

## Requisites

To use this scripts the following packages are needed:
* vmdebootstrap
* bash
* wget
* xargs
* getopt
* sudo 

## How to use

	./rbp_img_build [-h hostname] [-r filesystem_root_type] [-p password] [-d distribution_name] [-m mirror] [-i image_name] [-s image_size] [-k package_list]
		-h hotname          [default: raspberry] Hostname of the image.
		-r file_system_type [default: ext4] Root filesystem type.
		-p password         [default: raspberry] Root password.
		-d distribution_name [default: jessie] Debian distribution name.
		-m mirror           [default: http:/ftp.es.debian.org/debian] Mirror to use for download the distribution.
		-i image_name       [default: rbp2.img] Image file to generate.
		-s image_size       [default: 1024M] Image size.
		-k package_list     Comma separated package list to include in the image.
