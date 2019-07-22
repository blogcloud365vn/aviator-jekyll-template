---
title: /server/{instance_id}/console/
position: 2.4
type: get
description: Lấy thông tin đường dẫn console
content_markdown: |-
  API sử dụng để  hiển thị các thông tin của máy chủ ảo
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/{instance_id}/console/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "message": "string",
        "url": "example.com"
      }

    title: Response
    language: json
---