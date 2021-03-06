---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Disable Snapshot Copy
  version: 1.0.0
  description: |-
    Disables the automatic copying of snapshots from one region to another region for a
                specified cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisableLogging:
    get:
      summary: Disable Logging
      description: |-
        Stops logging information, such as queries and connection attempts, for the
                    specified Amazon Redshift cluster.
      operationId: disableLogging
      x-api-path-slug: actiondisablelogging-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster on which logging is to be stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging
  /?Action=DisableSnapshotCopy:
    get:
      summary: Disable Snapshot Copy
      description: |-
        Disables the automatic copying of snapshots from one region to another region for a
                    specified cluster.
      operationId: disableSnapshotCopy
      x-api-path-slug: actiondisablesnapshotcopy-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster that you want to
          disable copying of            snapshots to a destination region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---