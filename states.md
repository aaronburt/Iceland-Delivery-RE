### Out for delivery


```http
GET /order/details?t=HCIB612 HTTP/2
Host: grj1qa6opa.execute-api.eu-west-2.amazonaws.com
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:130.0) Gecko/20100101 Firefox/130.0
Accept: */*
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate, br, zstd
Referer: https://track.iceland.co.uk/
Origin: https://track.iceland.co.uk
Connection: keep-alive
Sec-Fetch-Dest: empty
Sec-Fetch-Mode: cors
Sec-Fetch-Site: cross-site
Priority: u=4
Pragma: no-cache
Cache-Control: no-cache
TE: trailers
```

```http
HTTP/2 200 
date: Sun, 27 Oct 2024 13:20:50 GMT
content-type: application/json
content-length: 507
access-control-allow-origin: https://track.iceland.co.uk
access-control-allow-credentials: true
apigw-requestid: AT8zTiwmLPEEP7A=
X-Firefox-Spdy: h2
```

```json
{
    "result": "OK",
    "delivery_status": "Out for delivery",
    "estimated_delivery_time": "13:46",
    "internal_job_id": "20241027-1230-1430-XXXXXXX-0578",
    "delivery_slot_start": "13:30",
    "delivery_slot_end": "14:30",
    "delivery_completed": false,
    "delivery_date": "2024-10-27",
    "delivery_time": "12:53:35",
    "delivery_vehicle_reg": "XXXXXXX",
    "delivery_stop": 7.0,
    "jobs_attempted": 4,
    "map_image": "data:image/jpeg;base64,[BASE64_ENCODED_IMAGE]"
}
```


### Delivered


```http
GET /order/details?t=HCIB612 HTTP/2
Host: grj1qa6opa.execute-api.eu-west-2.amazonaws.com
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:130.0) Gecko/20100101 Firefox/130.0
Accept: */*
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate, br, zstd
Referer: https://track.iceland.co.uk/
Origin: https://track.iceland.co.uk
Connection: keep-alive
Sec-Fetch-Dest: empty
Sec-Fetch-Mode: cors
Sec-Fetch-Site: cross-site
Priority: u=4
Pragma: no-cache
Cache-Control: no-cache
TE: trailers
```

```http
HTTP/2 200 
date: Sun, 27 Oct 2024 13:35:43 GMT
content-type: application/json
content-length: 436
access-control-allow-origin: https://track.iceland.co.uk
access-control-allow-credentials: true
apigw-requestid: AT8zTiwmLPEEP7A=
X-Firefox-Spdy: h2
```

```json
{
    "result": "OK",
    "delivery_status": "Completed",
    "delivery_status_reason": "",
    "estimated_delivery_time": "13:46",
    "internal_job_set_id": "20241027-1230-1430-XXXXXXX-0578",
    "delivery_slot_start": "13:30",
    "delivery_slot_end": "14:30",
    "delivery_completed": true,
    "delivery_date": "2024-10-27",
    "delivery_time": "13:53:02",
    "delivery_vehicle_reg": "XXXXXXX",
    "delivery_stop": 7.0
}
```