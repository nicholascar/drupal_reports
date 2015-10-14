# drupal_reports
CSIRO creates large scientific reports for the Australian government and other clients. This module contains code and configuration for Drupal 7 in order to make online reports.

csiro_internal_theme: 
   The drupal theme for the site which was taken from Sharon Tickell's depo. 

   Installation

   1. Install and enable the Zen theme
   2. Move the folder to <drupal directory>/sites/all/themes/csiro_internal_theme
   3. Enable the theme in admin/appearance
   
   Note: report.css contains all the styling for a report and if you change the name of a content type then you
   need to update it here.
   
tableofcontents: 
   Custom module that creates a table of contents for a report content type.

   Installation

   1. Move the folder to <drupal directory>/sites/all/modules/
   2. Enable the module.
   
   Note: Will only work after the drupal report site is installed because it adds to the report content type

datasetSource:
   Populates the selection field for report elements that contains a source with sources from 
   the sample dataset given. Loads the dataset website and grabs the name of each source and its
   GUID. The GUID is sent to the metadataexporter for citations and the result is displayed as a key
   for the selection field.
   
   1. Move the folder to <drupal directory>/sites/all/modules/
   2. Enable the module.
   
   Note: Will only work after the drupal report site is installed because it adds to report elements