# ![LOGO](logo.png) Personnel Data **flow**ground Connector

## Description

A generated **flow**ground connector for the Personnel Data API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/personio.de/personnel/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:42+03:00

## API Description

API for reading and writing personnel data incl. data about attendances and absences

## Authorization

Supported authorization schemes:
- API Key
## Actions

### This endpoint is responsible for fetching attendance data for the company employees. It is possible to paginate results, filter by period and/or specific employees. The result will contain a list of attendance periods, structured as defined here.

#### Input Parameters
* `start_date` - _required_ - First day of the period to be queried. It is inclusive, so the day specified as start_date will also be considered on the results
* `end_date` - _required_ - Last day of the period to be queried. It is inclusive, so the day specified as end_date will also be considered on the results.
* `employees` - _optional_ - A list of Personio employee identifiers to filter the results. Only those employees specified here will be returned.
* `limit` - _optional_ - Pagination attribute to limit how many attendances will be returned per page
* `offset` - _optional_ - Pagination attribute to identify which page you are requesting, by the form of telling an offset from the first record that would be returned.

### This endpoint is responsible for adding attendance data for the company employees. It is possible to add attendances for one or many employees at the same time. The payload sent on the request should be a list of attendance periods, in the form of an array containing attendance period objects.

### This endpoint is responsible for deleting attendance data for the company employees.

#### Input Parameters
* `id` - _required_ - ID of the attendance period to delete

### List Employees

### Employee

#### Input Parameters
* `employee_id` - _required_ - Numeric `id` of the employee

### Provides a list of available time-off types, for example 'Paid vacation', 'Parental leave' or 'Home office'

#### Input Parameters
* `limit` - _optional_ - Pagination attribute to limit how many records will be returned per page
* `offset` - _optional_ - Pagination attribute to identify which page you are requesting, by the form of telling an offset from the first record that would be returned.

### This endpoint is responsible for fetching absence data for the company employees. It is possible to paginate results, filter by period and/or specific employees. The result will contain a list of absence periods, structured as defined here.

#### Input Parameters
* `start_date` - _optional_ - First day of the period to be queried. It is inclusive, so the day specified as start_date will also be considered on the results
* `end_date` - _optional_ - Last day of the period to be queried. It is inclusive, so the day specified as end_date will also be considered on the results.
* `employees` - _optional_ - A list of Personio employee identifiers to filter the results. Only those employees specified here will be returned.
* `limit` - _optional_ - Pagination attribute to limit how many attendances will be returned per page
* `offset` - _optional_ - Pagination attribute to identify which page you are requesting, by the form of telling an offset from the first record that would be returned.

### This endpoint is responsible for adding absence data for the company employees.

### This endpoint is responsible for deleting absence period data for the company employees.

#### Input Parameters
* `id` - _required_ - ID of the absence period to delete

### Absence Period

#### Input Parameters
* `id` - _required_ - Numeric `id` of the absence period

## License

**flow**ground :- Telekom iPaaS / personio-de-personnel-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
