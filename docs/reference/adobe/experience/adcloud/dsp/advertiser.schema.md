
# DSP Advertiser Schema

```
https://ns.adobe.com/xdm/adcloud/dsp/advertiser
```

Adobe Advertising Cloud DSP Advertiser Details.

| [Abstract](../../../../../abstract.md) | [Extensible](../../../../../extensions.md) | [Status](../../../../../status.md) | [Identifiable](../../../../../id.md) | [Custom Properties](../../../../../extensions.md) | [Additional Properties](../../../../../extensions.md) | Defined In |
|----------------------------------------|--------------------------------------------|------------------------------------|--------------------------------------|---------------------------------------------------|-------------------------------------------------------|------------|
| Can be instantiated | Yes | Stable | No | Forbidden | Permitted | [adobe/experience/adcloud/dsp/advertiser.schema.json](adobe/experience/adcloud/dsp/advertiser.schema.json) |
## Schema Hierarchy

* DSP Advertiser `https://ns.adobe.com/xdm/adcloud/dsp/advertiser`
  * [Record Schema](../../../../behaviors/record.schema.md) `https://ns.adobe.com/xdm/data/record`
  * [Audit trail](../../../../datatypes/auditing/auditable.schema.md) `https://ns.adobe.com/xdm/common/auditable`


## DSP Advertiser Example
```json
{
  "@id": "12",
  "dsp:advertiserKey": "QEr8RnlYHwnG4KbFSQoA",
  "dsp:advertiserName": "Workday",
  "dsp:advertiserStatus": "Active",
  "dsp:advertiserUrl": "http://www.workday.com",
  "dsp:accountId": "377165",
  "repo:createDate": "2019-04-26T14:00:00+00:00",
  "repo:modifyDate": "2019-04-26T14:00:00+00:00"
}
```

# DSP Advertiser Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@id](#id) | `string` | Optional | [Record Schema](../../../../behaviors/record.schema.md#id) |
| [dsp:accountId](#dspaccountid) | `string` | Optional | DSP Advertiser (this schema) |
| [dsp:advertiserKey](#dspadvertiserkey) | `string` | Optional | DSP Advertiser (this schema) |
| [dsp:advertiserName](#dspadvertisername) | `string` | Optional | DSP Advertiser (this schema) |
| [dsp:advertiserStatus](#dspadvertiserstatus) | `enum` | Optional | DSP Advertiser (this schema) |
| [dsp:advertiserUrl](#dspadvertiserurl) | `string` | Optional | DSP Advertiser (this schema) |
| [repo:createDate](#repocreatedate) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#repocreatedate) |
| [repo:modifyDate](#repomodifydate) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#repomodifydate) |
| [xdm:createdByBatchID](#xdmcreatedbybatchid) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmcreatedbybatchid) |
| [xdm:modifiedByBatchID](#xdmmodifiedbybatchid) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmmodifiedbybatchid) |
| [xdm:repositoryCreatedBy](#xdmrepositorycreatedby) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmrepositorycreatedby) |
| [xdm:repositoryLastModifiedBy](#xdmrepositorylastmodifiedby) | `string` | Optional | [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmrepositorylastmodifiedby) |
| `*` | any | Additional | this schema *allows* additional properties |

## @id
### Identifier

A unique identifier for the record.

`@id`
* is optional
* type: `string`
* defined in [Record Schema](../../../../behaviors/record.schema.md#id)

### @id Type


`string`
* format: `uri-reference` ??? URI Reference (according to [RFC3986](https://tools.ietf.org/html/rfc3986))






## dsp:accountId
### Account Identifier

The identifier of the account associated with this advertiser.The same accountId can serve multiple advertisers in case it represents an advertising agency.

`dsp:accountId`
* is optional
* type: `string`
* defined in this schema

### dsp:accountId Type


`string`






## dsp:advertiserKey
### Advertiser Key

Unique external identifier for the advertiser.

`dsp:advertiserKey`
* is optional
* type: `string`
* defined in this schema

### dsp:advertiserKey Type


`string`






## dsp:advertiserName
### Advertiser Name

The name of the advertiser.

`dsp:advertiserName`
* is optional
* type: `string`
* defined in this schema

### dsp:advertiserName Type


`string`






## dsp:advertiserStatus
### Advertiser Status

Indicates the advertiser's status, whether it is active, inactive or deleted.

`dsp:advertiserStatus`
* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#dspadvertiserstatus-known-values).

### dsp:advertiserStatus Known Values
| Value | Description |
|-------|-------------|
| `Active` | Active |
| `Inactive` | Inactive |
| `Deleted` | Deleted |




## dsp:advertiserUrl
### Advertiser Url

Advertiser Url.

`dsp:advertiserUrl`
* is optional
* type: `string`
* defined in this schema

### dsp:advertiserUrl Type


`string`






## repo:createDate

The server date and time when the resource was created in the repository, such as when an asset file is first uploaded or a directory is created by the server as the parent of a new asset. The date time property should conform to ISO 8601 standard. An example form is "2004-10-23T12:00:00-06:00".

`repo:createDate`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#repocreatedate)

### repo:createDate Type


`string`
* format: `date-time` ??? date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))




### repo:createDate Example

```json
"2004-10-23T12:00:00-06:00"
```


## repo:modifyDate

The server date and time when the resource was last modified in the repository, such as when a new version of an asset is uploaded or a directory's child resource is added or removed. The date time property should conform to ISO 8601 standard. An example form is "2004-10-23T12:00:00-06:00".

`repo:modifyDate`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#repomodifydate)

### repo:modifyDate Type


`string`
* format: `date-time` ??? date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))




### repo:modifyDate Example

```json
"2004-10-23T12:00:00-06:00"
```


## xdm:createdByBatchID
### Created by batch identifier

The dataset files in Catalog which has been originating the creation of the record.

`xdm:createdByBatchID`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmcreatedbybatchid)

### xdm:createdByBatchID Type


`string`
* format: `uri-reference` ??? URI Reference (according to [RFC3986](https://tools.ietf.org/html/rfc3986))






## xdm:modifiedByBatchID
### Modified by batch identifier

The last dataset files in Catalog which has modified the record. At creation time, `modifiedByBatchID` is set as `createdByBatchID`.

`xdm:modifiedByBatchID`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmmodifiedbybatchid)

### xdm:modifiedByBatchID Type


`string`
* format: `uri-reference` ??? URI Reference (according to [RFC3986](https://tools.ietf.org/html/rfc3986))






## xdm:repositoryCreatedBy
### Created by user identifier

User ID of who created the record.

`xdm:repositoryCreatedBy`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmrepositorycreatedby)

### xdm:repositoryCreatedBy Type


`string`






## xdm:repositoryLastModifiedBy
### Modified by user identifier

User ID of who last modified the record. At creation time, `modifiedByUser` is set as `createdByUser`.

`xdm:repositoryLastModifiedBy`
* is optional
* type: `string`
* defined in [Audit trail](../../../../datatypes/auditing/auditable.schema.md#xdmrepositorylastmodifiedby)

### xdm:repositoryLastModifiedBy Type


`string`





