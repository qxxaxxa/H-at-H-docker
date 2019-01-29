# Hentai@Home on Docker

## Tags

`arm`: For arm32v6 arm32v7
`arm64`: For arm64v8
`x64/latest`: For x64(Linux)
`i386`: For x32(Linux)

I can't offer image for windows due to the limitation of the DockerHub's Autobuild system.

## Install

Replace `/DOWNLOAD_DIR` and `YOUR_CLIENT_KEY` with yours.

## Run command below:
	#Pull image
	sudo docker pull Disappear9/h-at-h

	#Create volume for caches and logs
	sudo docker volume create h-at-h_data
	
	#Run it
	sudo docker run -d --name h-at-h -p port:port -v h-at-h_data:/hath/data -v /DOWNLOAD_DIR:/hath/download -e HatH_KEY=YOUR_CLIENT_KEY Disappear9/h-at-h

