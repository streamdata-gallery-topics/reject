---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Reject Certificate Transfer
  version: 1.0.0
  description: Rejects a pending certificate transfer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RejectCertificateTransfer:
    get:
      summary: Reject Certificate Transfer
      description: Rejects a pending certificate transfer.
      operationId: rejectCertificateTransfer
      x-api-path-slug: actionrejectcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: rejectReason
        description: The reason the certificate transfer was rejected
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers
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