# A Nodejs backend to wrap zoomitable D3 treemap displaying directory storage statistics

A very basic nodejs angularjs site presents a dynamic D3 treemap displaying directory storage statistics calculated by the storagestats project which can be visited at there. The storagestats utility determine storage utilized under any first root directory across a configurable number of file types, rolling up utilization statistics directory by directory until all metrics are totaled in the root directory. This information is output in a storagestats CSV file format with one row for each directory. A separate convert_csv_2_flare utility converts the CSV file format into a flare json format usable by the D3 treemap. The convert_csv_2_flare only outputs one file type with the default being the total of all file types. The dynamic website takes as input from the web page which file output information is desired and makes a request to the node data factory which passes the parameters to the Python csv_2_flare utility and units the json back to the angular application.  The json also contains all valid file types available file types within its working storagestats CSV file.


## Prerequisites

There are not many prerequisites required to build and run this project, but you'll need the following:

* Node.js 4
* Node Package Manager
* Python 2.7

## Installation & Configuration


### Application

```
??? Install Python
```

```
Install pip requirements ???
```

```
npm install
```


```
node app.js
```

