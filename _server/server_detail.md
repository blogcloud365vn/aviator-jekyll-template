---
title: /server
position: 4.2
type: get
description: Hiển thị thông tin chi tiết của máy chủ ảo
content_markdown: |-
  API sử dụng để  hiển thị các thông tin của máy chủ ảo
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/{instance_id}/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
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

    title: Response
    language: json
---