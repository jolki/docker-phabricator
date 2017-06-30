# This is a fork of nasqueron/phabricator Docker image (https://github.com/nasqueron/docker-phabricator) with the following additions:

* ImageMagick will be installed
 
New environment variables:
Variable                            | Phabricator config variable          | Description
------------------------------------|--------------------------------------|------------
PHABRICATOR_ENABLE_GIF		        |files.enable-imagemagick              | If set, GIF animations are enabled
PHABRICATOR_ENABLE_YOUTUBE          |remarkup.enable-embedded-youtube      | If set, embedded youtube videos are enabled
PHABRICATOR_ENABLE_PROTOTYPE_APPS   |phabricator.show-prototypes           | If set, prototype applications will be anebled
PHABRICATOR_DISABLE_TEST_PLAN_FIELD |differential.require-test-plan-field  | If set, the test-plan-field will be disabled
PHABRICATOR_SAVE_FILES_ON_DISC      |storage.local-disk.path /var/files    | If set, files will be stored on the disk instead of in MySQL. Please also set the volume to a directory on your local disk to gain access to the stored files.

*Thanks to nasqueron/phabricator for this awsome Docker image!*

I will not be able to maintain this Docker image on a regular basis.
Please use this image on your own risk. 

Please refer to https://github.com/nasqueron/docker-phabricator for further informations regarding the original nasqueron/phabricator Docker image.

