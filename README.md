# Mormon Shrivel - Meetinghouse Map Data from LDS.org
In April 2023, I found a way to collect the data avilable on https://maps.lds.org. My hope is to take a snapshot of these data every few days to give a better perspective into the growth of The Corporation of the President of the Church of Jesus Christ of Latter-day Saints.

This repo contains 2 files that track Mormon church growth: meetinghouse.json and unit.json.

The meetinghouse.json file contains information about the meetinghouses that contain wards and stakes.

The `unit.json`` file contains information about the wards and stakes.

The format of the JSON files is unconventional, but it was done in this way to save on storage space.

Each line (besides the datestamp comments) contains two tab-delimited columns:

1. The change to a specific unit/meetinghouse ID.
2. The JSON data for each unit/meetinghouse ID.

The changes are either ADD, DELETE, or CHANGE. These changes are calculated based on the previous date (a basic diff was performed on the JSON objects).

## Disclaimer
It should be noted that LDS.org does NOT give consistent data. While I haven't been able to sift through all the data myself, I've noticed that some wards appear, disappear, and then reappear.
Because of this inconsistency, I am recommending that the timestamps that I add should not be used as a concrete measurement for when a ward or stake is opened or closed. There are created and updated dates on each unit, which may be more reliable.

Units in places like China and Hong Kong are not accurate because of privacy laws about religious congregrations (I think).

## Contact Info
For the safety of bishops within the Mormon corporation, contact information for the bishops has been removed. This data should only be used to track the Mormon growth/shrivel patterns.
