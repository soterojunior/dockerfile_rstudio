# Docker image RStudio



## Description

- The image has packages install, Latex RStudio, dplyr etc.

## Setup Dockerfile

1. Build the image:

   `docker build -t _name_image_ .`

2. Run an instance of the image, mounting the host directory:

   `docker run -v /Users/#{your_user}/rstudio:/home/rstudio -d -p 8787:8787 compmetagen/rstudio`

3. Determine the ip address of your machine:

   `docker-machine ip`

4. Using a web browser visit that address appended with the port (8787), e.g.:

  `192.168.99.100:8787`

5. You can now login using default username and password:

	User: `rstudio`
	Password: `rstudio`
