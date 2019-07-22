---
title: /api/v1/server/
position: 2.1
type: get
description: Hiển thị thông tin các máy chủ ảo sở hữu
content_markdown: |-
  API sử dụng để  hiển thị các các máy chủ ảo mà user sở hữu
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "count": 0,
        "next": "http://example.com",
        "previous": "http://example.com",
        "results": [
            {
              "instance_id": "string",
              "status": "string",
              "addresses": "string",
              "name": "string",
              "created": "2019-07-18T06:41:10Z",
              "expired": "2019-07-18T06:41:10Z",
              "ip_addresses": [
                "string"
              ],
              "region": "string"
            }
          ]
      }
    title: Response
    language: json
---