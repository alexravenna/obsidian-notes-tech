# Description
- The [[Docker]] implementation of a [[Container Image|container image]]
- Uses [[Unionfs]]
	- The top layer of an image is writeable
# Image Naming
- Format:
	- `[HOST[:PORT_NUMBER]/][NAMESPACE/]REPOSITORY`
		- `HOST`: `docker.io` is the default
		- `PORT_NUMBER`: for use if a hostname is provided
		- `NAMESPACE`: a user's or organization's name; `library` is default and used for Docker Official images
		-  `REPOSITORY`: the name of this specific image
- Image [[#Tags|tagging]] is used to set the name and additionally a version/variant
# Tags
- Tags are used to name and version images
- Optional; default is `latest`
- Done with the parameter `-t <TAG>` or `--tag <TAG>` for `docker build`
	- Example tag: `alexravenna/my-image:1.0.0`
		- This would set:
			- the `NAMESPACE` to `alexravenna`
			- the `REPOSITORY` to `my-image`
			- and the version to `1.0.0`
	- Without specifying a tag, the image will have no name, just an ID