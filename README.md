<snippet>
  <content><![CDATA[
# ${1:Acquia Interview Assignment - Jody Thigpen}

TODO: Write a project description

## Installation


Install the latest Acquia-Drupal build from http://www.acquia.com/downloads

Required Modules:  
 - Views  (https://www.drupal.org/project/views)
 - Features  (https://www.drupal.org/project/features)
 - Strongarm  (https://www.drupal.org/project/strongarm)
 - Chaos Tools  (https://www.drupal.org/project/ctools)
 - Content Access  (https://www.drupal.org/project/content_access)
 - Secure Site  (https://www.drupal.org/project/securesite)



- Feature installation

With each of the required modules installed, upload acquia_interview_assignment-7.x-1.0.tar feature to the /sites/all/modules/ directory, or a subdirectory within this location.

Login to the new Drupal 7 install as the site admin and go to Structure -> Features

Enable the feature, click the checkbox next to the name, and then save settings.



- Generate Users & Content

To generate test content go to Configuration -> Develepmont -> Generate Content and select only “Article”.  Choose the desired settings for number of articles, time of creation, etc.  Generate.

To generate test users go to Configuration -> Development -> Generate users and select the number of users you would like to create, only 1 is required for this demo.  Select “Feed User” under the roles to assign to the new users.  Generate.
* Note: Unless another tool is enabled to do so, the user password will need to be set to allow authentication to the feed. 


## Usage

Accessing the homepage as an unauthenticated user will show only the default Drupal 7 welcome page.

To access the secure feed login to the site with one of the generated user accounts that was given the “Feed User” role and navigate to: http://<yoursite>.com/feed

 - or - 

To access from the URL only or from an RSS reader use the following format in the URL string where “username” and “password” are replaced with the username and password of the generated user.

http://username:password@acq2.jtstage.com/feed



