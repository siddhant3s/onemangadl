INSTALLATION:
==The Quick and Dirty way==
Copy the onemangadl and BeautifulSoup.py to /usr/bin
     #:cd <onemangadl-direcotry>
     #:sudo cp onemangadl BeautifulSoup.py /usr/bin/

==Proper but long way==
1).	 Copy the onemangadl to /usr/bin
	      #:cd <onemangadl-directory?
	      #:sudo cp onemangadl /usr/bin
2).	 Install BeautifulSoup
	 #: wget http://www.crummy.com/software/BeautifulSoup/download/3.x/BeautifulSoup-3.0.8.1.tar.gz
	 #: tar -zxvpf BeautifulSoup-3.0.8.1.tar.gz
	 #: sudo python BeautifulSoup-3.0.8.1/setup.py install
	 #: sudo rm -rI BeautifulSoup-3.0.8.1 build BeautifulSoup-3.0.8.1.tar.gz
----------------------------------------------------------------------------------------------------------

This script downloads any manga (or multiple mangas) from http://www.mangareader.net/.
You just need to provide the URL of the first page of the manga (actually any page of the manga will do ). For example, if you want to Download `Death Note' from http://mangareader.net then you need to provide the URL http://www.mangareader.net/113-4017-1/death-note/chapter-1.html. (Note 1)

You can specify what all chapters to download with the -C flag.
Just specify a range like -C4-5,57-60,96  this will download chapters 4 to 5, 57 to 60 and chapter 96. Note that chapter number starts from 1. Chapter 1 will always be the first chapter. -C2 will download the second chapter and so on.
If this flag is not specified, all the chapters are downloaded

On Unix and Linux based platform, where wget is available, it is recommended to use the -w switch. This will call wget to download the images. It serves advantages like displaying a progress bar and resuming the download.

The -d switch specify in which directory the manga will be saved, if not specified, the script automatically guess a name based on the manga name. If two or more manga URLs are given, this flag is ignored.

-v stands for verbose. This will output extra information about the program execution.

-q stands for quiet mode. This will not output any information on the screen. Only incase of failure, it will display the error message

In case you are not using -w swtich (for wget), you may be interested in setting up the number of retries this script performs if an image cannot be downloaded in the first go. Use the -r switch for this: -r4 will try four times to downlaod an image, then it will move to the next image. Default is 3.


Example:
To download the first 3 chapters of `Death Note' on a *nix based system with wget, I would most probably use
$: onemangadl -C1-3 -w http://www.mangareader.net/113-4017-1/death-note/chapter-1.html

=Why is this script as onemangadl? Wasn't onemanga.com shut?=
This script was initially made to download the manga from onemanga.com. Read this blogpost http://yatantrika.co.cc/?p=109. Now the script is ported to mangareader.net. I still choose to keep the name as it is.