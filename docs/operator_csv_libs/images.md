Module operator_csv_libs.images
===============================

Classes
-------

`Image(name=None, image=None, deployment=None, container=None)`
:   Object to hold information about a container or related image
    
    Keyword Arguments:
        image {string}      -- Image 
        name {string}       -- Name as identified in spec.relatedImages or olm.relatedImage annotation
        deployment {string} -- Name of deployment(default: {None})
        container {string}  -- Name of container (default: {None})

    ### Methods

    `get_digest(self)`
    :   Returns image digest 
        
        Returns:
            [string] -- [digest in format <type>:<hash> ]

    `get_image(self)`
    :   Return the full image 
        
        Returns:
            [string] -- [Full image in format <repo>/<name>[@digest][:tag]]

    `get_image_name(self)`
    :   Returns the image name, stripped of repo and tag/digest
        
        Returns:
            [string] -- [Name]

    `get_image_repo(self)`
    :   Returns the image_repo section of the overall image
        
        Returns:
            [string] -- [image repo i.e. quay.io/myrepo]

    `get_olm_name(self)`
    :   Return the name of the image. Typically associated with olm.relatedImage and spec.relatedImages
        
        Returns:
            [string] -- [Name]

    `get_tag(self)`
    :   Get the tag associated with an image if known
        
        Returns:
            [string] -- [tag]

    `set_digest(self, digest)`
    :   Set image digest
        
        Arguments:
            digest {string} -- Digest in format <type>:<hash>

    `set_image_repo(self, repo)`
    :

    `set_tag(self, tag)`
    :   Set new tag for image. Will update self.image only if image is identified by tag, but not overwrite digest
        
        Arguments:
            tag {String} -- New tag to set