# Contribution Guide

## How to add a new podcast to the list

Please feel free to open a pull request if you know of a German tech podcast that is not mentioned here.  
If you're in doubt if a particular podcast is a good fit for the list, **don't open an issue, but create a pull request right away** because that's easier to handle. Thanks! :smiley:

### Criteria to be accepted

Each podcast on the list should be

- a podcast :smiley:
- published using RSS feed
- in German :de: :austria: :switzerland:

### Format

:warning: **The main [`README.md`](/README.md) is a rendered version of the data. Do not edit it manually.**

To add a new podcast, please create a `.yml` file in the [`/podcasts`](/podcasts) directory like `/podcasts/<podcast-name>.yml`. 
Feel free to check out a few other YAML files in that directory to see how it should look like.

| Field                        | Type               | Description                                                                                |
|------------------------------|--------------------|--------------------------------------------------------------------------------------------|
| name                         | string             | Name of the podcast                                                                        |
| website                      | string (url)       | Website (full URL) of the podcast                                                          |
| podcastIndexID               | integer            | ID of the podcast in the [PodcastIndex](https://podcastindex.org/)                         |
| rssFeed                      | string (url)       | RSS feed that is used to publish new podcast episodes                                      |
| spotify                      | string (url)       | Spotify link (full URL) of the podcast show                                                |
| description                  | string             | Description of the podcast (in German)                                                     |
| tags                         | array (of strings) | List of tags / focus themes                                                                |
| weekly_downloads_avg         | -                  | Average weekly downloads (substructure)                                                    |
| weekly_downloads_avg.value   | integer            | Number of the average weekly downloads                                                     |
| weekly_downloads_avg.updated | string (date)      | Date in format YYYY-MM-DD on when the "number of the average weekly downloads" was updated |

Finally, create a pull request with all your changes. 

**Thanks for helping out!** :tada:
