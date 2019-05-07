# ![LOGO](logo.png) DLx **flow**ground Connector

## Description

A generated **flow**ground connector for the DLx API (version 0.3.1).

Generated from: https://api.apis.guru/v2/specs/digitallinguistics.io/0.3.1/swagger.json<br/>
Generated at: 2019-05-07T17:40:14+03:00

## API Description

The Digital Linguistics (DLx) REST API

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Get all Languages

> Retrieves all the Languages that the authenticated user or client has permission to access.

*Tags:* `Language`

#### Input Parameters
* `continuation` - _optional_ - The `dlx-continuation` header is used to send a continuation token with the request, when retrieving the next page of results.
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifModifiedSince` - _optional_ - The `If-Modified-Since` header is used to retrieve only results modified since a given time. The value of this header must be a valid date string.
* `maxItemCount` - _optional_ - The `dlx-max-item-count` header is used to limit the number of results to a certain amount at a time (by default all results will be returned). If there are more results to be returned, a continuation token will also be sent in the `dlx-continuation` header.
* `public` - _optional_ - Set this parameter to `true` to include all publicly-accessible resources, not just those that the user is listed as an Owner, Contributor, or Viewer for.

### Add a new Language

*Tags:* `Language`

### Upsert (create or replace) a Language

> Creates a Language if it does not yet exist (i.e. if the resource does not have an `id` property yet), or replaces the existing Language resource if it does. Note that this replaces the *entire* Language. It is not a partial update.

*Tags:* `Language`

#### Input Parameters
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Delete a Language by ID

*Tags:* `Language`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Retrieve a Language by ID

*Tags:* `Language`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifNoneMatch` - _optional_ - If `If-None-Match` header is used with GET requests to check whether you already have the most up-to-date version of the resource, and therefore do not need the resource sent again. The value of the `If-None-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to reduce bandwidth.

### Perform a partial update on a Language

> Performs a partial update the Language whose ID is specified in the URL. If the Language object has an `id` property, is ignored in favor of the ID in the URL.

*Tags:* `Language`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Get all Lexemes for a Language

*Tags:* `Language` `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `continuation` - _optional_ - The `dlx-continuation` header is used to send a continuation token with the request, when retrieving the next page of results.
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifModifiedSince` - _optional_ - The `If-Modified-Since` header is used to retrieve only results modified since a given time. The value of this header must be a valid date string.
* `maxItemCount` - _optional_ - The `dlx-max-item-count` header is used to limit the number of results to a certain amount at a time (by default all results will be returned). If there are more results to be returned, a continuation token will also be sent in the `dlx-continuation` header.
* `public` - _optional_ - Set this parameter to `true` to include all publicly-accessible resources, not just those that the user is listed as an Owner, Contributor, or Viewer for.

### Add a new Lexeme to a Language

*Tags:* `Language` `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on

### Upsert (add or replace) a Lexeme

*Tags:* `Language` `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Delete a Lexeme by ID

*Tags:* `Language` `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Get a Lexeme by ID

*Tags:* `Language` `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifNoneMatch` - _optional_ - If `If-None-Match` header is used with GET requests to check whether you already have the most up-to-date version of the resource, and therefore do not need the resource sent again. The value of the `If-None-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to reduce bandwidth.

### Perform a partial update on a Lexeme

*Tags:* `Lexeme`

#### Input Parameters
* `languageID` - _required_ - The ID of the Language to perform the operation on
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Get all Lexemes

> Retrieve all Lexemes that the authenticated user has permission to access. Include a `languageID` query parameter to limit results to Lexemes from a particular Language.

*Tags:* `Lexeme`

#### Input Parameters
* `continuation` - _optional_ - The `dlx-continuation` header is used to send a continuation token with the request, when retrieving the next page of results.
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifModifiedSince` - _optional_ - The `If-Modified-Since` header is used to retrieve only results modified since a given time. The value of this header must be a valid date string.
* `languageID` - _optional_ - The ID of the Language to perform the operation on
* `maxItemCount` - _optional_ - The `dlx-max-item-count` header is used to limit the number of results to a certain amount at a time (by default all results will be returned). If there are more results to be returned, a continuation token will also be sent in the `dlx-continuation` header.
* `public` - _optional_ - Set this parameter to `true` to include all publicly-accessible resources, not just those that the user is listed as an Owner, Contributor, or Viewer for.

### Add a new Lexeme

> Add a new Lexeme. A `languageID` must be provided either as a query parameter, or as an attribute on the Lexeme body.

*Tags:* `Lexeme`

#### Input Parameters
* `languageID` - _optional_ - The ID of the Language to perform the operation on

### Upsert (add or replace) a Lexeme

> Upsert (add or replace) a Lexeme. A `languageID` must be provided either as a query parameter, or as an attribute on the Lexeme body.

*Tags:* `Lexeme`

#### Input Parameters
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.
* `languageID` - _optional_ - The ID of the Language to perform the operation on

### Delete a Lexeme by ID

*Tags:* `Lexeme`

#### Input Parameters
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

### Get a Lexeme by ID

*Tags:* `Lexeme`

#### Input Parameters
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `deleted` - _optional_ - Setting the `deleted` option to `true` will return results that have been marked for deletion, but not yet deleted from the database. Otherwise requests for a resource marked for deletion will return a 410 error.
* `ifNoneMatch` - _optional_ - If `If-None-Match` header is used with GET requests to check whether you already have the most up-to-date version of the resource, and therefore do not need the resource sent again. The value of the `If-None-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to reduce bandwidth.

### Perform a partial update on a Lexeme

> Perform a partial update on a Lexeme.

*Tags:* `Lexeme`

#### Input Parameters
* `lexemeID` - _required_ - The ID of the Lexeme to perform the operation on
* `ifMatch` - _optional_ - The `If-Match` header is used with PUT and DELETE requests to check whether you have the most up-to-date version of the resource before updating or deleting it. The value of the `If-Match` header is the ETag (`_etag`) property of the resource. It is recommended that your application use this header whenever possible to avoid data conflicts.

## License

**flow**ground :- Telekom iPaaS / digitallinguistics-io-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
